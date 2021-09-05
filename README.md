<h1>React portfolio</h1>
<h3>Technical requirements</h3>

* Personal GitHub account
* React web frontend
* Typescript template
* Functional React components
* CI/CD pipeline for GitHub pages

<h3>Workflow :</h3>

1. Create new GitHub Repository
    * Name the repo to portfolio, etc.
    * Do not use a hyphen in the repository name. (hyphen in the url breaks the gh-pages)
    * Use only lowercase letters in the repository name. (```create-react-app``` doesn't like uppercase letters)
    * See docs/github.md
3. Clone your new repository to local
4. Open the project folder in terminal
5. Create new React project with ```npx``` command.
    * ```npx create-react-app . --template typescript```
    * Once the React is initialized, test it by running command ```npm run start```
6. initialize the CI/CD pipeline
   * See docs/cicd
7. Commit your filechanges
