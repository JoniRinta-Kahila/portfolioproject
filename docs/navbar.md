<h1>Part 5. react-router-dom 2/2</h1>
<h3>Router Links</h3>

1. Create new folder `./src/components/navbar`
2. Inside the navbar folder, create component and style files `navbar.tsx`, `navbar.module.scss`
3. Initialize your navbar component with `fcr` snippet and import the style file in it.
4. In scss file, create a new style class `.container` and set inside of your navbar start div tsg to use it as attribute.
5. Between the div tags, add three Link components, and for each link give `to` attribute to point your links to the `/`, `first` and `example` pages
    * `<Link to="/">Home</Link>` `<Link to="first">My First Component</Link>`
6. In index file, set your Navbar component between the BrowserRouter and Router elements.
