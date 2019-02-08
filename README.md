# Penn Labs Frontend Challenge

The frontend challenge for this semester is to build a product called Penn Course Cart in React! The goal of this challenge is for you to demonstrate:

1. An eye for building intuitive, feature-rich user interfaces
2. Ability to build products with minimal direction
3. Ability to work within a set timeline

More concretely, you will build an interface where users can explore computer science courses added at Penn, can add them to a cart, and checkout.

--------------------

### Getting started

* Fork this repository to your own GitHub account
* Clone the repository to your own computer
* `cd` into the cloned directory and run either `yarn` or `npm install`
* Run `yarn start` or `npm run dev`

--------------------

### General structure

```
public/
  index.html           Root HTML file for each page

src/                   Where the JS logic is
  components/          Contains all React components
    Cart.js            Basic component for the course cart
    Courses.js         Basic component for rendering courses
    Nav.js             Basic component for the navbar
    ...                Feel free to add other components

  data/                Contains data rendered by the components
    courses.json       Contains information on CIS courses at Penn


  App.css              CSS for the app
  App.js               Root component for the app
  index.js             Renders the React app
  ...
```

--------------------

### Features

1. __Explore courses__
  * If you view `src/components/Courses.js`, you'll see that it is rendering *some* of the courses data from `src/data/courses.json`
  * What you need to do is design a more robust way to display this courses information. You should display all information contained in the JSON--though put some thought into how to go about doing this.
    * For example, you might only want to show the description once the user clicks on the course.

2. __Add courses to your cart__
  * A user should be able to add a subset of these courses to their cart.
    * The user should not be able to add more than 7 courses to their cart.
  * When a user adds a course, this addition should be reflected in:
    1. How that cart is rendered
    2. How that course is rendered
      * For example, there should not still be a button to add that course to the cart, and maybe the text should be grayed out.

3. __View cart and checkout__
  * The user should be able to click a button to view their cart.
    * If the cart has no items in it, tell the user that their cart is empty.
    * If the cart has courses it in, display the courses and relevant information about them.
  * When the user is satisfied with their course cart, they should be able to "checkout"
    * This will either take the user to a new page containing (or will display on the same page) a "receipt" containing the courses which they checked out with.

4. __Additional features__
  * Feel free to add other features as well! Here are some ideas:
    * Integrate other data (course times, when they're offered, etc.)
      * For example, ping the Penn Labs API

```
fetch(https://api.pennlabs.org/registrar/search?q=cis-110)
```

    * Add animations for adding and viewing courses and the cart
    * Let users rank courses in order of preference
    * Allow users to filter and sort courses by different metrics

--------------------

### Additional tips

* For styling, use whatever you want:
  * CSS frameworks (Bulma, Bootstrap)
  * CSS files (or SCSS)
  * CSS-in-JS
  * `styled-components`
  * ...

* For state management:
  * Vanilla react state and props
  * Redux
  * ...

* For navigation:
  * React Router
  * ...

--------------------

### Getting help

If you have any questions about the project or need some help, send an email to __Cameron Cabo__ (ccabo@seas.upenn.edu) or message him on [Facebook](https://www.facebook.com/cam.cabo).
