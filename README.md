# React-Conceptual-Questions

1.  ## What is react?
    _**React**_ is a JavaScript library created by **<span style="color:#2D88FF;">Facebook</span>**. It is use for creating User Interface(UI). In react we can create complex UI by creating many small `components` and combining them.
    ***
2.  ## Differentiate between functional and class components. ## What do you prefer to use and in which situation?
    ***
3.  ## What is State and Props in react?

    _`State`_ is data maintained inside a component. It is owned by that specific component. The component itself will update the state using the setState function or hook.

    _`Props`_ is data passed in from a parent component. props are read-only in the child component that receives them. We need to pass callback functions, which can be executed inside the child to update **props**.

    ***

4.  ## What is the difference between State and Props? How do you decide what is controlled by state and what is controlled by pros?

    The difference is all about which component owns the data. **`State`** is owned locally and updated by the component itself. **`Props`** are owned by a parent component and are read-only.

    If data is shared with other components then we should use **props** else we should use **state**.

    ***

5.  ## What is Virtual DOM and how it works?

    The `virtual DOM` is only a virtual representation of the DOM. Everytime the state of our application changes, the virtual DOM gets updated instead of the real DOM. Like the actual DOM, the Virtual DOM is a node tree that lists elements and their attributes and content as objects and properties.

    Updation of DOM in react is 3 step process:-

    1.  Whenever anything may have changed, The entire virtual DOM gets re-rendered.
    2.  The difference between the Virtual DOM representation and a virtual DOM `snapshot` that was taken right before the update will be calculated.
    3.  The real DOM will be updated with what has actually changed.

    ***

6.  ## What is the importance of Key in the map?

    The `Keys` help **<span style="color:#2D88FF;">React</span>** identify which items have been changed added, or removed. Elements inside the array must be keyed to give a static identity to the elements. Most of the time we use object's `id` as a key. If id is not available then only we use array index. But we should try not to use an index as a key.

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

8.  ## Which life- cycle method will you use when calling an API?
    ***
9.  ## How do we access the parent component in a child and vice versa. ## (in react)
    ***
10. ## Have you used Context?
    ***
11. ## How to connect react with backend?
    ***
12. ## Why use Redux in react?
    ***
13. ## Explain how to work with redux?
    ***
14. ## What is the container pattern?
    ***
15. ## What is middleware used for?
    ***
