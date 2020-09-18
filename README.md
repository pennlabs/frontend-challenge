# Frontend Challenge: Fall '20

Welcome to the Penn Labs Frontend Challenge!

If you have already done this challenge, there's a [section below](#repeat-applicants) for you. 

In this challenge, you will be building a product called Penn Course Cart in React! The goal of this challenge is for you to demonstrate:

1. An eye for building intuitive, feature-rich user interfaces
2. Ability to build products with minimal direction
3. Ability to work within a set timeline

More concretely, you will build an interface where users can explore computer science courses added at Penn, can add them to a cart, and checkout.

## Getting Started

1. Copy this [repository](https://github.com/pennlabs/frontend-challenge) to your own GitHub account by clicking the green "use this template" button. You will have to make a Github account if you don't already have one. **Be sure to create a private repository.** **You will be submitting a ZIP file at the end of the technical.**
2. [Clone](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository) the repository you just made to your own computer. 

```bash
git clone https://github.com/pennlabs/frontend-challenge.git
```

3. Make sure you have [Node](https://www.seas.upenn.edu/~cis197/development) installed.

4. Navigate to the cloned directory in the command line and run `yarn` or `npm install`

5. Run `yarn start` or `npm start`

**Note:** This project is bootstrapped with [Create React App (CRA)](https://github.com/facebook/create-react-app), so hot-reloading has been configured. This means after you run `yarn start` or `npm start`, the application will be recompiled automatically after a file is edited. 

## General Structure

We have provided minimal starter code with the following structure. 

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

## Features

Your application should implement the following features. 

1. **Explore Courses**

    If you view `src/components/Courses.js`,  you'll see that it is rendering some of the courses data from `src/data/courses.json` What you need to do is design a more robust way to display this courses information. You should display all information contained in the JSON — though put some thought into how to go about doing this. For example, you might only want to show the description once the user clicks on the course.

    In addition, a user should be able to filter or sort courses by particular properties such as keywords in course descriptions, prerequisites etc.

2. **Add courses to your cart**
    - A user should be able to add a subset of these courses to their cart. Further, The user should not be able to add more than 7 courses to their cart.
    - When a user adds a course, this addition should be reflected in:
        - How that cart is rendered
        - How that course is rendered (e.g. there should not still be a button to add that course to the cart, and maybe the text should be grayed out)
3. **View cart**
    - The user should be able to click a button to view their cart.
        - If the cart has no items in it, tell the user that their cart is empty.
        - If the cart has courses in it, display the courses and relevant information about them.
4. **Additional Features** 

    Feel free to add other features as well! Here are some ideas:

    - Big bonus if you integrate other data (course times, when they're offered, etc.). A great resource is the [Penn Labs API](https://github.com/pennlabs/labs-api-server). Let us know if you need an API key,
    - Add Typescript ([https://create-react-app.dev/docs/adding-typescript/](https://create-react-app.dev/docs/adding-typescript/)) to your application. Kudos if you turn on `strictNullChecks` and `noImplicitAny`!
    - Allow users to "checkout" their current cart, which takes the user to a new page (React Router/next.js could be useful here!) containing a "receipt" with the courses they checked out with.
    - Add animations for adding and viewing courses and the cart
    - Let users rank courses in order of preference
    - Thinking about code quality: take advantage of a [linter](https://eslint.org/).

## Additional Tips

- For styling, use whatever you want:
    - CSS frameworks (Bulma, Bootstrap)
    - CSS files (or SCSS)
    - CSS modules
    - CSS-in-JS
    - `styled-components`
- For state management, you have several options:
    - Vanilla react state, props and [context managers](https://reactjs.org/docs/context.html)
    - [Redux](https://redux.js.org/)
    - [SWR](https://swr.vercel.app/)
- For navigation:
    - React Router

### **Getting help**

If you have any questions about the project or need some help, send an email to **Daniel Tao** ([dtao@seas.upenn.edu](mailto:dtao@seas.upenn.edu)) or message him on [Facebook.](https://www.facebook.com/danieltaox/)

### **Repeat applicants**

First off, thanks so much for your continued interest in Labs. We've accomplished a lot in the past year and have plans for more great products and features which need new developers to tackle them—so fingers crossed!

At Labs we don't just build new products, we also maintain legacy code bases and year over year push out new and improved versions. [Penn Course Review](https://penncoursereview.com/) and the [Common Funding Application](https://penncfa.com/) are two great examples.

In line with this, we want you to take your submission from when you last applied, clean up your code, and take it to the next level with new features and data. Be deliberate with your implementation decisions, architecture, and documentation such that if someone else opens your code 6 months from now they'll be able to pick up right where you left off. We're excited to see what you come up with.

## Submission

You should have created a private copy of the template repository we gave you. To get a ZIP file that you can submit on the submission form, push all your code to GitHub, click the green "Code" dropdown, and then click "Download ZIP". You can then upload this to our submission form.