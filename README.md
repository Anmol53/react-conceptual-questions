# React-Conceptual-Questions

1.  ## What is react?

    _**React**_ is a JavaScript library created by **<span style="color:#2D88FF;">Facebook</span>**. It is used to create a User Interface(UI). In react we can create complex UI by creating and combining many small `components`.

    ***

2.  ## Differentiate between functional and class components. What do you prefer to use and in which situation?

    _**Functional Component:**_ It's just a function which accepts props and returns a React component. It uses react hooks to manipulate data. There are many react hooks. Like, useState(), useEffect(), etc.

    _**Class Component:**_ We use ES6 class syntax to write component. We need to extend `React.Component` to create a component. We have to use life-cycle methods to manipulate the data in the class component, according to the phase of the component.

    Both versions are equivalent and will give you the exact same output.

    I like to use `Functional Component`. Initially, Functional Component did not have the capabilities as much as `Class Component`. Like update state and other life cycle methods. But after the v16.8 update of React, we can also do all those things in Functional Component using hooks.

    I prefer Functional Component because it is simpler to write, less complex than Class Component, and has all the functionality as Class Component.

    ***

3.  ## What are State and Props in react?

    The _`State`_ is data maintained inside a component. It is owned by that specific component. The component itself will update the state using the setState function or useState hook.

    The _`Props`_ is data passed in from a parent component. props are read-only in the child component that receives them. We need to pass callback functions, which can be executed inside the child to update **props**.

    ***

4.  ## What is the difference between State and Props? How do you decide what is controlled by state and what is controlled by pros?

    The difference is all about which component owns the data. **`State`** is owned locally and updated by the component itself. **`Props`** are owned by a parent component and are read-only.

    If data is shared with other components then we should use **props** else we should use **state**.

    ***

5.  ## What is Virtual DOM and how it works?

    The `virtual DOM` is only a virtual representation of the DOM. Every time the state of our application changes, the virtual DOM gets updated instead of the real DOM. Like the actual DOM, the Virtual DOM is a node tree that lists elements and their attributes and content as objects and properties.

    Updation of DOM in **<span style="color:#2D88FF;">React</span>** is 3 step process:-

    1.  Whenever anything may have changed, The entire virtual DOM gets re-rendered.
    2.  The difference between the Virtual DOM representation and a Virtual DOM `snapshot` that was taken right before the update will be calculated.
    3.  The real DOM will be updated with what has actually changed.

    ***

6.  ## What is the importance of Key in the map?

    The `Keys` help **<span style="color:#2D88FF;">React</span>** identify which items have been changed added, or removed. Elements inside the array must be keyed to give a static identity to the elements. Most of the time we use an object's `id` as a key. If id is not available then only we use array index. But we should try not to use an index as a key.

    ***

7.  ## What are the life- cycle methods in react?

    Each component in **<span style="color:#2D88FF;">React</span>** has a lifecycle consist of three main phases.
    The three phases are: `Mounting`, `Updating`, and `Unmounting`.

    - **Mounting** phase Lifecycle methods:

      1. constructor()
      2. getDerivedStateFromProps()
      3. render()
      4. componentDidMount()<br><br>

    - **Updating** phase Lifecycle methods

      1.  getDerivedStateFromProps()
      2.  shouldComponentUpdate()
      3.  render()
      4.  getSnapshotBeforeUpdate()
      5.  componentDidUpdate()<br><br>

    - **Unmounting** phase Lifecycle methods
      1.  componentWillUnmount()

    ***

8.  ## Which life-cycle method will you use when calling an API?

    If API call is not dependent upon state or props data than we will use `componentDidMount()`.

    `componentDidUpdate()` is used when API call is dependent on state or props data.

    ***

9.  ## How do we access the parent component in a child and vice versa. (in react)

    We can access the parent component's data in a child component using `props`. The data which parent data is passing via props will be available in child component.

    We have to use the `callback function` to access the child component's data in the parent component.

    ***

10. ## Have you used Context?

    In a `React` application, data is passed top-down (parent to child) via props, but it becomes tedious when data is required by many components within an application. `Context` provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree. Context is primarily used when some data needs to be accessible by many components at different nesting levels.

    Context is designed to share data that can be considered "global" for a tree of React components, such as the current authenticated user, theme, etc.

    The benefit of using Context:

    - We can avoid passing props through intermediate elements.
    - Code becomes simple.

    ***

11. ## How to connect react with backend?

    We need to set `proxy` to backend URL in `package.json` file. Like: `"proxy": "http://localhost:8080"`. And than we can make API Calls to this URL to perform any operations on backend.

    ***

12. ## Why use Redux in react?

    When multiple components require the same data, we need to `lift the state up` until we find the common ancestor. We know that in React, data can only flow in one direction `(top-down)`. Therefore, we will also need to create multiple callbacks to update the data. This will cause two problems. First, data will also be available to the intermediate components, even if the data is not required by them. Second, the code becomes too complex. Therefore we use _`Redux`_.

    _`Redux`_ is a state management library. Redux helps manage the global state of an application by creating a global store. From this store, any component can access the store's data and update the data.

    ***

13. ## Explain how to work with redux?

    ***

14. ## What is the container pattern?

    ***

15. ## What is middleware used for?

    ***
