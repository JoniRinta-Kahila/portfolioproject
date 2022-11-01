<h1>Visual Studio Code Snippets</h1>

Code snippets are templates that make it easier to enter repeating code patterns, speeding up your code writing. In Visual Studio Code, snippets appear in IntelliSense (Ctrl+Space) mixed with other suggestions.

"You can easily define your own snippets without any extension. To create or edit your own snippets, select User Snippets under - Code/File > Preferences > Configure User Snippets > New Global Snippets file..."
https://code.visualstudio.com/docs/editor/userdefinedsnippets#_create-your-own-snippets


1. Create a new code snippet in Visual Studio Code - Code/File > Preferences > Configure User Snippets - and name it to ```react.code-snippets```
2. Paste the following snippet script in react.code-snippets file & save it.
3. Test the script by writing ```fcr``` to a new tsx file and press enter.

The following snippet is very useful when creating new react components. 

```code-snippets
{
  "Functional Component": {
    "prefix": "fc",
    "body": [
      "import React from 'react'",
      "",
      "type $1Props = {",
      "",
      "}",
      "",
      "const $1: React.FC<$1Props> = () => (",
      "  <div>",
      "    ${1:${TM_FILENAME_BASE/(.*)/${1:/capitalize}/}}",
      "  </div>",
      ")",
      "",
      "export default $1",
      ""
    ],
    "description": "React functional component"
  },
  "Functional Component return": {
    "prefix": "fcr",
    "body": [
      "import React from 'react'",
      "",
      "type $1Props = {",
      "",
      "}",
      "",
      "const $1: React.FC<$1Props> = () => {",
      "  return (",
      "    <div>",
      "      ${1:${TM_FILENAME_BASE/(.*)/${1:/capitalize}/}}",
      "    </div>",
      "  )",
      "}",
      "",
      "export default $1",
      ""
    ],
    "description": "React functional component with return"
  },
}
```
