# REACT

React.js, also known as React, is an open-source JavaScript library that is used to build user interfaces. It's primarily used for developing single-page applications and allows developers to create reusable UI components.

React.js is a component-based front-end library that is responsible only for the view layer of a Model View Controller (MVC) architecture. This means that it's used to create the part of our application that interacts with the user.

React.js uses a declarative paradigm that makes applications both effective and flexible. It creates simple views for each state in our application and efficiently updates and renders just the right components as our data changes. The declarative view makes our code more predictable and easier to debug.

Each component in a React application is responsible for rendering a separate, reusable piece of HTML code. The ability to nest components within other components allows we to build complex applications from simple building blocks. A component can also keep track of its internal state, for example, a TabList component can hold a variable for the open tab in memory.

React.js was initially developed and maintained by Facebook and later used in its products like WhatsApp & Instagram
. While building client-side applications, a team of Facebook developers found that the Document Object Model (DOM) was slow. To make it faster, React implements a virtual DOM which is basically a DOM tree representation in JavaScript.

React.js is updated frequently, with new features being added with each version. The current stable version of React.js is 18.2.0 and was released on June 14, 2022.

React.js works by creating a virtual DOM in memory to update the browser’s DOM. The virtual DOM will try to find the most efficient way to update the browser’s DOM. Unlike browser DOM elements, React elements are simple objects and are cheap to create. React DOM takes care of updating the DOM to match the React elements.

---

## Conditional rendering

Conditional rendering in React is a technique that allows us to render different components or elements based on certain conditions. It works the same way conditions work in JavaScript. You can use JavaScript operators like `if` or the conditional operator to create elements representing the current state, and let React update the UI to match them.

For example, if we have a `PackingList` component rendering several `Item`s, which can be marked as packed or not, we can write this as an `if / else` statement like so:

```jsx
function Item({ name, isPacked }) {
  if (isPacked) {
    return <li className = "item">{name} ✔ </li>;
  }
  return <li className = "item">{name}</li>;
}
```

If the `isPacked` prop is true, this code returns a different JSX tree. With this change, some of the items get a checkmark at the end.

In some situations, we might not want to render anything at all. For example, say you don’t want to show packed items at all. A component must return something. In this case, we can return `null`:

```jsx
function Item({ name, isPacked }) {
  if (isPacked) {
    return null;
  }
  return <li className = "item">{name}</li>;
}
```

If `isPacked` is true, the component will return nothing (`null`). Otherwise, it will return JSX to render.

In practice, returning `null` from a component isn’t common because it might surprise a developer trying to render it. However, it's a powerful tool when you need it. This is just one of many ways that conditional rendering can be used in React.

1. **React - Lists & Keys**: In React, you often need to display a list of data. This is done by creating multiple components and rendering them using JavaScript's `map()` function. Each item in the list should have a unique "key" prop, which helps React identify which items have been added, changed, or removed.

2. **React - Forms**: Forms in React are similar to regular HTML forms, but with some differences. The form data is typically handled by the state within a component, and changes to the input fields are handled by events⁵⁶. This allows for more control and customization of form behavior.

3. **React - Lifting State**: Lifting state up is a technique in React where you share state data between multiple components. Instead of keeping state local within one component, you "lift" the state up to a parent component, which can then distribute it to its children[^10^]. This helps keep your state logic in one place and allows multiple components to share and manipulate the same data.

4. **React - Composition vs Inheritance**: React has a powerful composition model, and it's recommended to use composition instead of inheritance to reuse code between components. In other words, instead of creating a complex hierarchy of components where properties are inherited from parent to child, you can create smaller, simpler components and combine them together (or "compose" them) to create more complex UIs.

5. **Thinking in React**: This is a mindset or approach to building applications in React. It involves breaking down your application into separate components based on UI and functionality, thinking about the minimal representation of the application state, identifying where the state should live in the component hierarchy, and adding data flow across the components.
