### HTML Questions

### 1. What is HTML?
HTML (Hypertext Markup Language) is the standard language used to create and design web pages. It structures content on the web using various tags and attributes.

### 2. What are the different types of HTML tags?
HTML tags can be classified into:
- **Structural tags**: `<html>`, `<head>`, `<body>`, `<header>`, `<footer>`.
- **Content tags**: `<h1>`, `<p>`, `<a>`, `<img>`, `<ul>`, `<li>`.
- **Form tags**: `<form>`, `<input>`, `<textarea>`, `<button>`.
- **Metadata tags**: `<meta>`, `<title>`, `<link>`, `<style>`.

### 3. What is the difference between `<div>` and `<span>` tags?
- `<div>` is a block-level element used to structure or group larger sections of content.
- `<span>` is an inline element used for smaller portions of content, often for styling or grouping text within a block element.

### 4. What is the `alt` attribute in the `<img>` tag?
The `alt` attribute provides alternative text for an image when it cannot be displayed. It is important for accessibility and SEO.

### 5. What are semantic HTML tags?
Semantic HTML tags clearly describe their meaning in a human-readable way. Examples include `<article>`, `<section>`, `<nav>`, `<header>`, and `<footer>`, which help improve accessibility and SEO.

### 6. What is the purpose of the `doctype` declaration in HTML?
The `doctype` declaration defines the document type and version of HTML, helping the browser to render the document correctly.

### 7. What is the difference between inline and block elements?
- **Block elements**: These elements take up the full width of their container, e.g., `<div>`, `<h1>`, `<p>`.
- **Inline elements**: These elements take up only the necessary width and flow inline with other content, e.g., `<span>`, `<a>`, `<strong>`.

### 8. What are forms in HTML?
Forms in HTML are used to collect input from users. They consist of various form elements like text fields, checkboxes, radio buttons, and submit buttons.

---

### CSS Questions

### 9. What is CSS?
CSS (Cascading Style Sheets) is used to style and format the layout of a web page, including its colors, fonts, and spacing.

### 10. What are the different ways to apply CSS to a webpage?
CSS can be applied in three ways:
- **Inline CSS**: Using the `style` attribute directly within HTML tags.
- **Internal CSS**: Placing CSS rules within the `<style>` tag in the HTML document’s `<head>`.
- **External CSS**: Linking to an external CSS file using the `<link>` tag.

### 11. What is the box model in CSS?
The box model defines how the layout of elements on a webpage is structured. It consists of:
- **Content**: The actual content inside the element.
- **Padding**: Space between the content and the border.
- **Border**: The border surrounding the element.
- **Margin**: Space outside the border.

### 12. What is the difference between `class` and `id` selectors in CSS?
- `class`: A selector that can be used to apply styles to multiple elements.
- `id`: A selector that is unique and can only be used for one element on a page.

### 13. What are pseudo-classes in CSS?
Pseudo-classes are used to define the special states of an element, such as `:hover`, `:focus`, or `:nth-child`. They help in styling elements based on user interactions or document structure.

### 14. What is Flexbox in CSS?
Flexbox is a layout model that allows elements to be arranged in rows or columns with flexible spacing. It helps create responsive layouts easily by distributing space dynamically between elements.

### 15. What is the difference between `position: relative`, `absolute`, and `fixed`?
- **Relative**: The element is positioned relative to its normal position.
- **Absolute**: The element is positioned relative to the nearest positioned ancestor.
- **Fixed**: The element is positioned relative to the viewport and stays fixed even when the page is scrolled.

### 16. What is CSS Grid?
CSS Grid is a two-dimensional layout system that enables you to design complex grid-based layouts with rows and columns.

### 17. What is a media query in CSS?
Media queries are used to apply different styles depending on the device's characteristics, such as screen size, resolution, or orientation.

---

### JavaScript Questions

### 18. What is JavaScript?
JavaScript is a high-level, interpreted programming language used to create interactive effects and dynamic content on websites.

### 19. What is the difference between `var`, `let`, and `const` in JavaScript?
- `var`: Declares a variable with function or global scope (not block-scoped).
- `let`: Declares a block-scoped variable that can be reassigned.
- `const`: Declares a block-scoped constant that cannot be reassigned.

### 20. What are functions in JavaScript?
A function is a block of reusable code that performs a specific task. It can take inputs (parameters) and return outputs (results).

### 21. What is the difference between `null` and `undefined` in JavaScript?
- `null`: Represents the intentional absence of any value or object.
- `undefined`: Represents a variable that has been declared but not assigned a value.

### 22. What are JavaScript events?
JavaScript events are actions that occur in response to user interactions, such as clicks, keypresses, or mouse movements. They are used to trigger specific functions when a particular event happens.

### 23. What is a promise in JavaScript?
A promise is an object that represents the eventual completion (or failure) of an asynchronous operation. It allows handling asynchronous code more easily by chaining `then()` and `catch()` methods.

### 24. What are arrow functions in JavaScript?
Arrow functions are a shorthand syntax for writing functions in JavaScript. They do not have their own `this` context and are often used for cleaner code.

### 25. What is the difference between `==` and `===` in JavaScript?
- `==` checks for equality of values, performing type coercion if necessary.
- `===` checks for equality of both value and type, without type coercion.

### 26. What are callbacks in JavaScript?
A callback is a function that is passed as an argument to another function and is executed after the first function completes its operation.

### 27. What is DOM in JavaScript?
DOM (Document Object Model) represents the HTML structure of a webpage as an object, allowing JavaScript to manipulate the content, structure, and style of a webpage dynamically.

### 28. What are closures in JavaScript?
A closure is a function that retains access to its lexical scope, even when it is executed outside that scope. Closures help create private variables in JavaScript.


### 29. What is Hoisting in JavaScript?
Hoisting is a JavaScript mechanism where variables and function declarations are moved to the top of their containing scope during the compile phase. This means variables can be used before they are declared.

### 30. What is a JavaScript Module?
A module in JavaScript is a piece of code that is encapsulated and can be exported and imported to share functionality between files. JavaScript modules help organize code into smaller, reusable pieces.

### 31. What is the `this` keyword in JavaScript?
The `this` keyword refers to the object that is executing the current function. It can have different values depending on the context in which it is used.

### 32. What is event delegation in JavaScript?
Event delegation is a technique in JavaScript where a single event listener is attached to a parent element, rather than to individual child elements. This approach allows for handling events on dynamically added elements.

### 33. What is JSON (JavaScript Object Notation)?
JSON is a lightweight data interchange format that is easy for humans to read and write, and easy for machines to parse and generate. It is used to send and receive data between a server and a client in JavaScript.

### 34. What is the difference between `call()`, `apply()`, and `bind()` in JavaScript?
- **`call()`**: Invokes a function with a given `this` value and arguments passed individually.
- **`apply()`**: Similar to `call()`, but arguments are passed as an array.
- **`bind()`**: Creates a new function that, when called, has its `this` value set to a specified object, and arguments can be pre-set.

### 35. What is an Immediately Invoked Function Expression (IIFE)?
An IIFE is a function expression that is defined and executed immediately after its creation. It is often used to create a local scope to avoid polluting the global namespace.

### 36. What is the difference between synchronous and asynchronous programming in JavaScript?
- **Synchronous**: Code is executed line by line, blocking the execution of other tasks until the current one completes.
- **Asynchronous**: Code execution doesn't block other operations, allowing tasks to run concurrently (e.g., using callbacks, promises, or async/await).

### 37. What is `localStorage` and `sessionStorage` in JavaScript?
- **`localStorage`**: Stores data with no expiration time, persisting even after the browser is closed.
- **`sessionStorage`**: Stores data for the duration of the page session, which is cleared when the page is closed.

### 38. What are template literals in JavaScript?
Template literals are string literals that allow embedded expressions, multi-line strings, and easier string interpolation using backticks (`` ` ``) instead of quotes.

### 39. What is the `setTimeout()` function in JavaScript?
`setTimeout()` is a JavaScript function that executes a specified function after a certain delay (in milliseconds).

### 40. What is the `setInterval()` function in JavaScript?
`setInterval()` is a JavaScript function that repeatedly executes a specified function at regular intervals (in milliseconds).

### 41. What is the `forEach()` method in JavaScript?
The `forEach()` method is used to iterate over elements in an array, executing a provided function once for each element in the array.

### 42. What is the difference between `map()` and `forEach()` in JavaScript?
- **`map()`**: Returns a new array by applying a function to each element of the array.
- **`forEach()`**: Executes a function on each element of the array but does not return anything.

### 43. What is the `filter()` method in JavaScript?
The `filter()` method creates a new array with all elements that pass a test specified by a provided function.

### 44. What is the `reduce()` method in JavaScript?
The `reduce()` method applies a function to each element in an array (from left to right) to reduce it to a single value, such as summing numbers or concatenating strings.

### 45. What are promises in JavaScript?
Promises are objects that represent the eventual completion or failure of an asynchronous operation. They allow chaining of `.then()` and `.catch()` to handle success and failure cases.

### 46. What is the `async/await` syntax in JavaScript?
`async/await` provides a more readable way to work with promises. `async` marks a function as asynchronous, and `await` pauses the execution until the promise resolves.

### 47. What is `NaN` in JavaScript?
`NaN` stands for "Not-a-Number." It is a special value representing an invalid or undefined numerical result (e.g., dividing zero by zero).

### 48. What is the difference between `window` and `document` objects in JavaScript?
- **`window`**: Represents the global window object that contains properties like `location`, `history`, and `alert()`. It is the top-level object in the browser environment.
- **`document`**: Represents the HTML document, providing methods to access and manipulate elements within the web page.

### 49. What is the difference between `undefined` and `not defined` in JavaScript?
- **`undefined`**: A variable is declared but not assigned a value.
- **`not defined`**: A variable has not been declared at all.

### 50. What is event bubbling in JavaScript?
Event bubbling is a mechanism in the DOM where an event starts from the innermost element and propagates outward to the outermost element. It allows handling events at higher levels in the DOM tree.

### 51. What is the difference between `slice()` and `splice()` in JavaScript?
- **`slice()`**: Returns a shallow copy of a portion of an array without modifying the original array.
- **`splice()`**: Changes the contents of an array by removing, replacing, or adding elements in place.

### 52. What is `NaN` and how to check it?
`NaN` stands for "Not-a-Number" and is returned when a mathematical operation cannot be performed. To check if a value is `NaN`, you can use the `Number.isNaN()` method.

### 53. What is a JavaScript callback function?
A callback function is a function that is passed as an argument to another function and is executed after the first function completes its task.

### 54. What is `const` in JavaScript?
`const` is used to declare variables that are read-only and cannot be reassigned. It is block-scoped and must be initialized with a value during declaration.


