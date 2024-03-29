<h1>React portfolio</h1>

[Open part 2 (SASS) =>](sass)

[Back to clean Web version, click here](https://jonirinta-kahila.github.io/portfolioproject/)

<h3>Technical requirements</h3>

* Personal GitHub account
* Responsive React web frontend
* Typescript template
* Functional React components
* SASS (syntactically awesome style sheets)
* CI/CD pipeline for GitHub pages

<h3>Workflow :</h3>

<h4>Initialize project</h4>

1. Create new <b>GitHub Repository</b>. [Click to create new repository](https://github.com/new)
    * Name the repo to e.g. <b>portfolio</b>.
    * Set repo to <b>Public</b>.
    * <strong style="color: red">Do not use a hyphen (-) in the repository name.</strong> (hyphen in the url breaks the gh-pages)
    * Use only lowercase letters in the repository name.
    <!-- * See [docs/github.md](https://github.com/JoniRinta-Kahila/portfolioproject/blob/main/docs/github.md) -->
3. Clone your new repository to local
    * Open <b>cmd or terminal</b> in the file path of your choice
    * Run command ```git clone [link to your git-repo]```
5. **Open the project folder in terminal**
6. Create a new React project with ```npx``` command.
    * ```npx create-react-app@latest . --template typescript```
         * <strong style="color: red">Warning! If there comes a warning about vulnerabilities, DON'T try to fix them using any - <b>Audit fix</b> - commands, since those errors will not affect to your final React app, but fixing breaks the current React version. </strong>
    * Once the React is initialized, test it by running command ```npm run start```
    * If everything works as expected, the browser will open and you will see the react logo in it.
7. Initialize the CI/CD pipeline
   * See <b>[docs/cicd](https://github.com/JoniRinta-Kahila/portfolioproject/blob/main/docs/cicd.md)</b>
8. Commit your filechanges, then push.
   * ```git status``` show list of your project status
   * ```git add .``` add any new or modified files to the index.
   * ```git commit -m "commit message"``` make changes locally. Add a comment describing the changes
   * ```git push``` push your saved changes to the server

<h4>Start creation with TypeScript</h4>

1. The first step is to open the project in **Visual Studio Code** and delete unnecessary files from the project. Delete the following files
      * <b>src/App.css</b>
      * <b>src/index.css</b>
      * <b>src/logo.svg</b>
2. Open <b>index.tsx</b> file and remove imports from deleted files.
3. Open <b>App.tsx</b> file
4. Replace all contents in <b>App.tsx</b> with

```tsx
// App.tsx
import React from 'react'
import MyFirstComponent from './components/myFirstComponent';

const App: React.FC = () => {
  return (
    <div>
      <MyFirstComponent />
    </div>
  )
}

export default App
```
5. Now the error ```Cannot find module './components/myFirstComponent' or its corresponding type declarations.``` appear
      * To fix it, create a folder at the ```./src``` and name it to ```components```
      * Create new file ```myFirstComponent.tsx``` in ```./src/components```

6. In the ```./src/components/myFirstComponent.tsx``` paste next code in it and save.

```tsx
import React from 'react'

type MyFirstComponentProps = {

}

const MyFirstComponent: React.FC<MyFirstComponentProps> = () => {
  return (
    <div>
      <h1>Hello, React!</h1>
      <p>This is my first component 😎</p>
    </div>
  )
}

export default MyFirstComponent

```

7. Run command ``npm run start`` again to see the changes.

8. Visual Studio Code Snippets
      * Snippets help you write code faster.
      * See [docs/snippets](https://github.com/JoniRinta-Kahila/portfolioproject/blob/main/docs/snippets.md)
9. Remember to commit & push your code changes to github!
   * ```git status``` show list of your project status
   * ```git add .``` add any new or modified files to the index.
   * ```git commit -a -m "commit message"``` make changes locally. Add a comment describing the changes
   * ```git push``` push your saved changes to the server

<h3>Documentations</h3>

* [TypeScript docs](https://www.typescriptlang.org/docs/)
* [React docs](https://reactjs.org/docs/hello-world.html)

## [Open part 2 (SASS) =>](sass)
