<h1>Part-2. Add Dart sass to project</h1>

<h3>Workflow</h3>

1. Install <b>Dart Sass npm</b> package
     * Open commandline at the root of the project (Your project root is the same folder where your <b>package.json</b> file is.)
     * use command ```npm install sass```
2. Create example component
   * Create a new folder in ``./components``. Name folder to ``example``
   * Create a new file ``someExampleComponent.tsx`` in ``./components/example``
   * Create a new file inside a ``./components/example`` and name it to ``someExampleComponent.module.scss``
   * Open the <b>someExampleComponent.tsx</b> file and use your ``fcr`` code snippet and save.
        * see [docs/snippets](https://github.com/JoniRinta-Kahila/portfolioproject/blob/main/docs/snippets.md)
   * Import style file, placing ```import styles from './someExampleComponent.module.scss'``` to the top of the <b>someExampleComponent.tsx</b>
   * Replace all HTML in your example components return statement with HTML code at the end of this file.
        * You can see the ```className={styles.container}``` part in ``div`` element, it is a style reference to the style class of the sass file you imported.
    * Paste style class from end of this file to your components style file.
    * Now open <b>App.tsx</b> file and import this example component.
        * ```import SomeExampleComponent from './components/example/someExampleComponent'```
    * Now you can use this new component, just like HTML!
        * in <b>App.tsx</b>, place ``<SomeExampleComponent />`` between divs.
3. Now you can check the results, run command ``npm run start``again
4. Remember to commit & push the project to the GitHub.
    
<h4>HTML</h4>

```html
<div className={styles.container}>
  <h1>Header</h1>
  <p>My supercool component</p>
</div>
```

<h4>CSS / SCSS</h4>

```sass
.container {
  width: 100%;
  height: 450px;
  background: #1abc9c;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  h1 {
    font-size: 52px;
    color: azure;
    text-shadow: 2px 2px #7860ff;
  }

  p {
    font-weight: 700;
    font-size: 25px;
    color: rgb(206, 255, 255);
    background: rgb(255, 0, 200);
    padding: 10px;
  }
}
```

## [<-- BACK TO PART 1](/portfolioproject) ...... [GO TO PART 3 (HOOKS) -->](usestate)
