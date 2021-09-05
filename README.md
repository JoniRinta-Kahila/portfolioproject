<h1>React portfolio</h1>
<h3>Technical requirements</h3>

* Personal GitHub account
* React web frontend
* Typescript template
* Functional React components
* SASS (syntactically awesome style sheets)
* CI/CD pipeline for GitHub pages

<h3>Workflow :</h3>

<h4>Initialize project</h4>

1. Create new GitHub Repository
    * Name the repo to portfolio, etc.
    * Do not use a hyphen in the repository name. (hyphen in the url breaks the gh-pages)
    * Use only lowercase letters in the repository name. (```create-react-app``` doesn't like uppercase letters)
    * See [docs/github.md](https://github.com/JoniRinta-Kahila/portfolioproject/blob/main/docs/github.md)
3. Clone your new repository to local
4. Open the project folder in terminal
5. Create new React project with ```npx``` command.
    * ```npx create-react-app . --template typescript```
    * Once the React is initialized, test it by running command ```npm run start```
    * If everything works as expected, the browser will open and you will see the react logo in it.
6. initialize the CI/CD pipeline
   * See [docs/cicd](https://github.com/JoniRinta-Kahila/portfolioproject/blob/main/docs/cicd.md)
7. Commit your filechanges, then push.

<h4>Start creation with TypeScript</h4>

