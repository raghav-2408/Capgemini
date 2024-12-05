### 1. What is React.js?
React.js is an open-source JavaScript library used for building user interfaces, particularly for single-page applications. It allows developers to create reusable UI components and manage the view layer of applications.

### 2. What is JSX?
JSX (JavaScript XML) is a syntax extension for JavaScript that allows you to write HTML-like code within JavaScript. React uses JSX to describe what the UI should look like.

### 3. What are components in React?
Components are the building blocks of a React application. They can be either class-based or function-based and are used to define the structure and behavior of the UI.

### 4. What is the difference between a class component and a functional component?
- **Class component**: Uses ES6 class syntax and has access to lifecycle methods and state management.
- **Functional component**: A simpler function-based component that doesn't have access to lifecycle methods or state unless using React hooks (introduced in React 16.8).

### 5. What are props in React?
Props (short for properties) are read-only attributes passed from parent to child components. They allow components to communicate with each other by passing data.

### 6. What is state in React?
State is an object used to store dynamic data in a component. It can be changed over time, and when the state changes, the component re-renders to reflect the updated state.

### 7. What are React hooks?
React hooks are functions that allow you to use state and other React features in functional components. Common hooks include `useState`, `useEffect`, `useContext`, etc.

### 8. What is the `useState` hook?
The `useState` hook is used to add state to functional components. It returns an array with two elements: the current state value and a function to update the state.

### 9. What is the `useEffect` hook?
The `useEffect` hook is used to perform side effects in functional components, such as fetching data, subscribing to a service, or manually updating the DOM. It runs after the component renders.

### 10. What are controlled components in React?
A controlled component is a component where form data is controlled by React's state. The input element's value is managed by the state, and updates are triggered through event handlers.

### 11. What are uncontrolled components in React?
An uncontrolled component is a component where form data is handled by the DOM itself. React does not manage the state directly, and instead, you access the form values using `ref`.

### 12. What is the virtual DOM in React?
The virtual DOM is a lightweight copy of the real DOM. React uses it to optimize rendering by updating only the necessary parts of the real DOM when changes occur, rather than re-rendering the entire DOM.

### 13. What is Redux?
Redux is a predictable state container for JavaScript apps, often used with React. It helps manage the state of an application in a centralized store, allowing components to access and update the state in a consistent way.

### 14. What is the purpose of `key` in React lists?
The `key` prop is used to identify which items in a list are changed, added, or removed. It helps React efficiently update and render only the changed elements, improving performance.

### 15. What is React Router?
React Router is a library used to handle routing in a React application. It enables navigation between different views or pages without reloading the entire page, supporting single-page applications (SPAs).

### 16. What is the difference between `componentDidMount` and `useEffect`?
- **`componentDidMount`** is a lifecycle method used in class components to perform tasks after the component has been rendered to the DOM.
- **`useEffect`** is a hook used in functional components for similar purposes but with more flexibility, such as running on component mount, update, or unmount.

### 17. What is the `context` API in React?
The `context` API is used to manage and share state across the component tree without having to pass props manually at every level. It's useful for passing global data like themes or user authentication.

### 18. What is the difference between `React.Fragment` and `<div>`?
`React.Fragment` is used to group multiple elements without adding an extra node to the DOM. It is often used when you need to return multiple elements but do not want to wrap them in a `div`.

### 19. What is the purpose of `React.StrictMode`?
`React.StrictMode` is a wrapper component that helps identify potential problems in an application during development. It does not affect the production build but can highlight issues like unsafe lifecycle methods and deprecated APIs.

### 20. What are Higher-Order Components (HOCs) in React?
Higher-Order Components (HOCs) are functions that take a component and return a new component with additional props or functionality. They are used for code reuse and logic abstraction.
