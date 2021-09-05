<h1>CI/CD pipeline</h1>

<h3>Term</h3>

* The main concepts attributed to CI/CD are continuous integration, continuous delivery, and continuous deployment.
    * CI => Continuous Integration
    * CD => Continuous Delivery & Deployment


<h3>Continuous integration</h3>
Continuous integration means an automated testing process. A successful CI leads to the transition of new code changes to the production.

<h3>Continuous Deployment</h3>
Continuous deployment (CD) mean the automatic releasing of changes made by the developers, from the development version to production, where it is available to customers.

<h3>Workflow</h3>

1. To add CI/CD pipeline to your project, create a ```.github/workflows/``` folder at the root of the project.
2. Create ```BuildAndDeploy.yml``` file in ```./.github/workflows```
3. Paste next code in the ```BuildAndDeploy.yml```

```yml
name: Build and Deploy
on: [push]
jobs:
  build-and-deploy:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout 🛎️
        uses: actions/checkout@v2.3.1

      - name: Install and Build 🔧 # This example project is built using npm and outputs the result to the 'build' folder. Replace with the commands required to build your project, or remove this step entirely if your site is pre-built.
        run: |
          npm install
          npm run build
      - name: Deploy 🚀
        uses: JamesIves/github-pages-deploy-action@4.1.3
        with:
          branch: gh-pages # The branch the action should deploy to.
          folder: build # The folder the action should deploy.
```
