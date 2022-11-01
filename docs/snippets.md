<h1>Visual Studio Code Snippets</h1>

Code snippets are templates that make it easier to enter repeating code patterns, speeding up your code writing. In Visual Studio Code, snippets appear in IntelliSense (Ctrl+Space) mixed with other suggestions.

"You can easily define your own snippets without any extension. To create or edit your own snippets, select User Snippets under File > Preferences (Code > Preferences on macOS), and then select the language (by language identifier) for which the snippets should appear, or the New Global Snippets file option if they should appear for all languages. VS Code manages the creation and refreshing of the underlying snippets file(s) for you."
https://code.visualstudio.com/docs/editor/userdefinedsnippets#_create-your-own-snippets


1. Create a new code snippet in Visual Studio Code (Ctrl/Command + Shift + P) and name it to ```react.code-snippets```
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
