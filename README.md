![CF](http://i.imgur.com/7v5ASc8.png) LAB
=================================================

<!-- LINKS -->
<!-- Replace the link for each in brackets below -->
<!-- PR (working into submission) -->
[1]: https://github.com/401-advanced-javascript-billybunn/lab-26/pull/1
<!-- travis build -->
[2]: https://www.travis-ci.com/YOUR_ORG_NAME/REPO_NAME
<!-- back-end -->
[3]: http://xyz.com
<!-- front-end -->
[4]: https://codesandbox.io/s/4wxqjz24jx
<!-- swagger -->
[5]: http://xyz.com
<!-- jsdoc-->
[6]: heroku-link/docs 

## Component Based UI

### Author: Billy Bunn

### Links and Resources
* [PR][1]
<!-- * [travis][2] -->
<!-- (when applicable) -->
<!-- * [back-end][3] -->
<!-- (when applicable) -->
* [Code Sandbox][4]

#### Documentation
<!-- API assignments only -->
<!-- * [swagger][5] -->
<!-- (All assignments) -->
<!-- * [jsdoc][6] -->

### Modules
#### `index.js`
Entry point for the React application. Requires React and React DOM as dependencies, so it can render content to the page. Contains the `Main` React class component, i.e., `class Main` extends the `React.Component` class and uses its `render()` function to return `<App />`.

Everything rendered through index.js is rended to the DOM in the `#root` div in `index.html`.

#### `app.js`

##### `Counter` React class component. 
* `Counter` has a constructor function that takes `props`—the React component properties—as a parameter. The constructor also contains the `state` of the `Counter` component, a property that tracks the current number on the counter displayed in the DOM.

The `Counter` class component has three methods:
   * `decrement` - takes an `event` object as a parameter and changes the `state` of `Counter` to a number one less than the current `state` (using `this.setState`).
   * `increment` - identical to `decrement`, but instead increases the current state by one.
   * `render` - defines the markup rendered to the DOM: two `<a>` tags (for decrementing and incrementing) and a `<h4>` containing the current count. This is an inherited method from `React.Component`

##### `App` React class component
* `App` uses its inherited `render()` method to return the three main components as markup: `Header`, `Counter`, and `Footer`.

#### `header.js`
React class component containing markup for the header.

#### `footer.js`
React class component containing markup for the footer.

#### `app.scss`
Sass CSS styling for the entire application.

#### UML
![UML Diagram](https://i.imgur.com/1wN8scu.jpg)
