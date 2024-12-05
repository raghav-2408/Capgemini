### Node.js

#### 1. What is Node.js?
Node.js is an open-source, cross-platform JavaScript runtime built on Chrome's V8 engine that allows JavaScript to be run server-side. It enables developers to use JavaScript for both client-side and server-side scripting.

#### 2. What is npm in Node.js?
npm (Node Package Manager) is a package manager for JavaScript. It is used to install, share, and manage dependencies in Node.js applications. npm provides a large number of open-source libraries and tools.

#### 3. What are callbacks in Node.js?
Callbacks in Node.js are functions that are passed as arguments to other functions and are executed when a certain task is completed. They help handle asynchronous operations without blocking the execution flow.

#### 4. What are Streams in Node.js?
Streams in Node.js are used to handle large amounts of data efficiently. They allow reading or writing data in chunks rather than all at once, which improves performance, especially when dealing with files or networks.

#### 5. What is Express.js in Node.js?
Express.js is a minimal and flexible Node.js web application framework that simplifies the creation of server-side applications. It provides methods for routing, handling requests, and working with middleware.

#### 6. What is the event loop in Node.js?
The event loop is the core mechanism that handles asynchronous operations in Node.js. It allows non-blocking I/O operations by executing tasks in the background while keeping the main thread free.

#### 7. What is middleware in Node.js?
Middleware is a function in Express.js that is executed during the lifecycle of a request. It can modify the request and response objects, execute code, or terminate the request-response cycle.

#### 8. What is asynchronous programming in Node.js?
Asynchronous programming allows tasks to be executed concurrently, preventing blocking operations. Node.js uses non-blocking, event-driven architecture to handle multiple requests simultaneously.

---

### EJS (Embedded JavaScript)

#### 9. What is EJS?
EJS (Embedded JavaScript) is a templating engine that lets you embed JavaScript into HTML pages. It allows you to dynamically generate HTML content by using variables and loops.

#### 10. How does EJS work?
EJS works by embedding JavaScript code inside HTML using `<% %>` tags. The server processes the EJS file, and the final HTML content is sent to the client.

#### 11. What is the difference between EJS and other templating engines?
EJS allows you to write plain HTML with embedded JavaScript, making it simple and easy to understand. Other templating engines like Handlebars or Pug might require more specialized syntax and rules.


#### 12. How do you pass data from a Node.js application to EJS templates?
You can pass data to EJS templates using the `render()` method in your Express.js route. This data can be in the form of variables, arrays, or objects, which EJS will use to generate dynamic content.

#### 13. How do you include partials in EJS?
You can include partials in EJS using the `<%- include 'partial_name' %>` syntax. This allows you to reuse common parts of the HTML structure, such as headers, footers, or navigation bars.

#### 14. What is the use of `<%= %>` in EJS?
The `<%= %>` syntax is used to output the value of a variable or expression into the HTML content. For example, `<%= user.name %>` will print the name property of the `user` object.

#### 15. What is the difference between `<% %>` and `<%= %>` in EJS?
- `<% %>`: Executes JavaScript code without printing anything to the output.
- `<%= %>`: Executes JavaScript code and outputs the result to the HTML.

---

### Socket.io

#### 16. What is Socket.io?
Socket.io is a JavaScript library that enables real-time, bi-directional communication between web clients and servers. It is commonly used for creating real-time web applications such as chat apps, live updates, or multiplayer games.

#### 17. How does Socket.io work?
Socket.io works by establishing a WebSocket connection between the client and server, allowing both to send and receive messages instantly. It automatically falls back to long-polling when WebSockets are not supported.

#### 18. What is the difference between WebSocket and Socket.io?
- **WebSocket**: A protocol that provides full-duplex communication channels over a single, long-lived connection.
- **Socket.io**: A library built on top of WebSocket that provides additional features like automatic reconnection, broadcasting, and fallback options when WebSocket is not available.

#### 19. How do you establish a connection in Socket.io?
In Socket.io, a connection is established between the client and server using `socket.emit()` on the client side and `socket.on()` on the server side. Once the connection is established, both can communicate by emitting and listening for events.

#### 20. What are namespaces in Socket.io?
Namespaces in Socket.io are used to divide the communication channels into multiple segments. Each namespace can have its own set of event listeners and emitters, providing logical separation for different parts of the application.

#### 21. What are rooms in Socket.io?
Rooms in Socket.io are a way to group clients within a namespace. They allow for targeted messaging, enabling the server to emit messages to specific rooms of users (e.g., sending a message to all users in a chat room).

#### 22. What is broadcasting in Socket.io?
Broadcasting in Socket.io refers to sending messages to all clients except the sender. It is commonly used in applications like chatrooms, where you want all users to receive updates except the user who sent the message.

#### 23. What is the purpose of `socket.emit()` in Socket.io?
`socket.emit()` is used to send messages from the server to the client. You can specify the event name and the data you want to send along with the message.

#### 24. What is the purpose of `socket.on()` in Socket.io?
`socket.on()` is used to listen for specific events from the server or client. It executes a callback function whenever an event is emitted.

#### 25. How do you handle disconnections in Socket.io?
Socket.io automatically handles disconnections, but you can listen for the 'disconnect' event on the server side to perform specific actions when a client disconnects, such as cleaning up resources or updating the status.

