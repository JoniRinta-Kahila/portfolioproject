<h1>Part 6. react-router-dom 2/2</h1>
<h3>Router Links</h3>

1. Create new folder `./src/components/navbar`
2. Inside the navbar folder, create component and style file for it `navbar.tsx`, `navbar.module.scss`
3. Initialize your <b>navbar</b> component with `fcr` snippet and import the style file in it.
4. In the <b>navbar.module.scss</b>, create a new style class `.container` and call it inside of your <b>navbar.tsx</b> start div tag to use it as an attribute. (See [Part-2. Add Dart sass to project](sass))
5. Between the div tags, add three Link components, and for each link give `to` attribute to point your links to the `/`, `first` and `example` pages
    * `<Link to="/">Home</Link>` `<Link to="first">My First Component</Link>`
6. In the index file, set your Navbar component between the BrowserRouter and Router elements.

## [<-- BACK TO PART 5 (ROUTER)](router) ...... [GO TO PART 7 (PROJECT) -->](portfolio)
