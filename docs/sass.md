<h1>Part-2. Add node-sass to project</h3>

<h3>Workflow</h3>

1. Install node-sass npm package
    * Open commanddline at the root of the project (Your project root is the same folder where your package.json file is.)
    * use command ```npm install node-sass```
2. Create example component
    * Create a new folder in ``./components``. Name folder to ``example``
    * Create a new file ``someExampleComponent.tsx`` in ``./components/example``
    * Create a new file inside a ``./components/sassExample`` and name it to ``someExampleComponent.module.scss``
    * Open the someExampleComponent.tsx file and use your ``fcr`` code snippet and save.
        * see [docs/snippets](https://github.com/JoniRinta-Kahila/portfolioproject/blob/main/docs/snippets.md)
    * Import style file, placing ```import styles from './example.module.scss'``` to the top of the ``someExampleComponent.tsx``
    * Replace all HTML in your example components return statement with HTML code at the end of this file.
        * You can see the ```className={styles.container}``` part in ``div`` element, it is a style reference to the style class of the sass file you imported.
    
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
   height 450px;
   background: #1abc9c;
}
```
