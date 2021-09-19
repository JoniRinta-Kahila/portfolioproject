<h1>create-react-app</h1>

1. Create new GitHub Repository using [this template link](https://github.com/JoniRinta-Kahila/portfolioproject/generate)
    * Name the repo to portfolio, etc.
    * Set repo to public.
    * Do not use a hyphen in the repository name. (hyphen in the url breaks the gh-pages)
    * Use only lowercase letters in the repository name.
    <!-- * See [docs/github.md](https://github.com/JoniRinta-Kahila/portfolioproject/blob/main/docs/github.md) -->
3. Clone your new repository to local
    * Open cmd or terminal in the file path of your choice
    * Run command ```git clone [link to your git-repo]```
5. **Open the project folder in terminal**
6. Create new React project with ```npx``` command.
    * ```npx create-react-app . --template typescript```
    * Once the React is initialized, test it by running command ```npm run start```
    * If everything works as expected, the browser will open and you will see the react logo in it.
7. Initialize the CI/CD pipeline
   * See [docs/cicd](https://github.com/JoniRinta-Kahila/portfolioproject/blob/main/docs/cicd.md)
8. Commit your filechanges, then push.
   * ```git status``` show list of your project status
   * ```git add .``` add any new or modified files to the index.
   * ```git commit -a -m "commit message"``` make changes locally. Add a comment describing the changes
   * ```git push``` push your saved changes to the server
