<h1>Part 4. react-router-dom</h1>

<h3>react-router-dom is a collection of navigational components.</h3>

These components allows us to develope a single-page web application with navigation without re-rendering the page during user navigation. These components calls the necessary components to display the required information in the application.

<h3>Install react-router-dom npm package</h3>

1. Open a commandline at the root of the project.
2. Run command ``npm install react-router-dom@5.2.1``
    * ``@5.2.1`` represents the package version
3. Run command ``npm i --save-dev @types/react-router-dom``
    * Sometimes we need to install package types too
    * ``--save-dev`` flag mark package to the dev dependencies. the dev dependencies are not included in the build.

<h3>Import react-router-dom</h3>

1. Open App.tsx
2. Import react-router-dom components

```tsx
import {
  BrowserRouter as Router,
  Switch,
  Route,
  Link
} from 'react-router-dom';
```

<h3>HTML</h3>
<b>Replace all the HTML in the component with the code below</b>

```html
    // Important! add your repositoryname to basename
    <Router basename='/YourRepoNameHere'>
      
      {/* The navigation bar and other components you want to display on all pages come here */}
      <div className={styles.navbar}>
        <Link to='/'>Front page</Link>
        <Link to='example'>Look my example component</Link>
      </div>

      <Switch>
        {/* Changing content comes here */}
        <Route exact path='/' component={MyFirstComponent} />
        <Route exact path='/example' component={SomeExampleComponent}/>
      </Switch>

      {/* The footer and other components you want to display on all pages come here */}
      <ClickCounter />

    </Router>
```

<h3>STYLES</h3>

1. Create new style file ``./src/App.module.scss``.
2. Create new styleclass ``body``,
      * set margin to 0.
3. Create new styleclass ``.navbar``,
      * in navbar class, set display to flex,
      * in navbar class, set flex-direction to column.
4. In App.tsx, import stylefile.
5. In HTML in App.tsx, set the correct style class for the navigation component.
6. In Router component, set basename to your repo name


## [<-- BACK TO PART 3](https://github.com/JoniRinta-Kahila/portfolioproject/blob/main/docs/usestate.md) ...... [GO TO PART 5 -->](https://github.com/)
