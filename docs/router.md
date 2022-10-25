<h1>Part 5. react-router-dom</h1>

<h3>react-router-dom is a collection of navigational components.</h3>

These components allows us to develope a single-page web application with navigation without re-rendering the page during user navigation. These components calls the necessary components to display the required information in the application.

<h3>Install react-router-dom npm package</h3>

1. Open a commandline at the root of the project.
2. Run command ``npm install react-router-dom@6.4.2``
    * ``@6.4.2`` represents the package version

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

1. Create new style file ``./src/App.module.scss``.
2. Create new styleclass ``body``,
      * set margin to 0.
3. Create new styleclass ``.navbar``,
      * in navbar class, set display to flex,
      * in navbar class, set flex-direction to column.
4. In App.tsx, import stylefile.
5. In Router component, set basename to your repo name

<h3>Documentations</h3>

[react-router-dom](https://reactrouter.com/web/guides/primary-components)

## [<-- BACK TO PART 4](https://github.com/JoniRinta-Kahila/portfolioproject/blob/master/docs/props.md) ...... [GO TO PART 5 -->](https://github.com/)
