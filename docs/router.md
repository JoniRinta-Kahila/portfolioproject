<h1>Part 5. react-router-dom 1/2</h1>

<h3>react-router-dom is a collection of navigational components.</h3>

These components allows us to develope a single-page web application with navigation without re-rendering the page during user navigation. These components calls the necessary components to display the required information in the application.

<h3>Install react-router-dom npm package</h3>

1. Open a commandline at the root of the project.
2. Run command ``npm install react-router-dom@6.4.2``
    * ``@6.4.2`` represents the package version
    * <strong style="color: red">Warning! If there comes a warning about vulnerabilities, DON'T try to fix them using any - <b>Audit fix</b> - commands, since those errors will not affect to your final React app, but fixing breaks the current React version. </strong>

<h3>Import react-router-dom</h3>

1. Open index.tsx
2. Import react-router-dom components

```tsx
import {
  BrowserRouter,
  Routes,
  Route,
} from "react-router-dom";
```

<h3>HTML</h3>
<b>Replace all the HTML in the component with the code below</b>

```html
   <React.StrictMode>
    <BrowserRouter>
      <Routes>
        <Route path='/' element={<App />}></Route>
        <Route path='example' element={<SomeExampleComponent />} />
        <Route path='/first' element={<MyFirstComponent />} />
      </Routes>
    </BrowserRouter>
  </React.StrictMode>
```

<h3>STYLES</h3>

1. Create new style file ``./index.module.scss``.
2. Create new styleclass ``body``,
      * set margin to 0.
3. In index.tsx, import index styles ``import ./index.module.scss``
4. Now you can test your new links `localhost:3000/`, `localhost:3000/example`, `localhost:3000/first`

<h3>Documentations</h3>

[react-router-dom]([https://reactrouter.com/web/guides/primary-components](https://reactrouter.com/en/v6.3.0/getting-started/overview))

## [<-- BACK TO PART 4](props) ...... [GO TO PART 6 (Navbar) -->](navbar)
