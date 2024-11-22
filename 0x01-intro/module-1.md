# Node.js Basics - Module 1

Welcome to the first step in my **Node.js** journey. In this module, I will get familiar with the basic concepts of **Node.js**, how to install and set it up on my environment, and then build my first script. By the end of this first module, I’ll understand what **Node.js** is, how it works, and why it’s great for building scalable server-side applications.

## What I will learn?

- Understand the definition of **Node.js** and its use cases.
- Set up my environment to run **Node.js** applications.
- Write and execute my first **Node.js** script.
- Comprehend how **Node.js** differs from browser JavaScript.
- Understand the core architecture of Node.js, including the event loop and its single-threaded nature.

## What I’ll Cover

### 1. What is Node.js?

#### Definition:

Node.js is a JavaScript runtime built on Chrome’s V8 JavaScript engine. It allows me to run JavaScript code outside the browser, enabling me to build server-side applications. Traditionally, JavaScript was only used on the client-side (in the browser), but Node.js extends JavaScript to the server-side.

#### Key Features of Node.js:

- **Non-blocking I/O**:
  Node.js uses a non-blocking, event-driven architecture that allows for handling many operations concurrently. It’s ideal for applications that require real-time data and multiple client connections (e.g., chat apps, live updates).

- **Single-threaded Event Loop**:
  Node.js runs on a single thread, using an event loop to handle multiple connections efficiently. This allows Node.js to handle thousands of concurrent requests without the overhead of thread management.

#### Why Node.js is Good for Servers:

- **Scalability**:
  Because of its non-blocking, event-driven nature, Node.js is highly scalable. It can handle numerous concurrent connections with minimal overhead, making it an excellent choice for building web servers, RESTful APIs, and real-time applications like messaging platforms.

- **Fast and Efficient**:
  Built on Chrome's V8 engine, Node.js is fast in executing JavaScript code. It also minimizes the number of threads and resources, making it more lightweight compared to traditional server-side technologies.

### 2. Installing Node.js

- To get started with **Node.js**, I will need to install it on my machine. I can easily find installation steps for my OS from the [Node.js Official Website](https://nodejs.org/en/download/package-manager)
- Verify Installation: Once installed, I’ll confirm it’s working by running these commands in my terminal:

  ```bash
  node -v
  npm -V
  ```

  This should display the installed version of **Node.js** and **NPM(Node Package Manager)**

### 3. First Steps with Node.js

- **Using the Node.js REPL (Read-Eval-Print Loop)**: The REPL allows me to quickly run JavaScript commands in the **Node.js** envirnoment:

  1. Start the REPL:

  ```bash
  node
  ```

  2. Print something cool:

  ```javascript
  > console.log("Here is something cool!")
  ```

- **Exiting the REPL**: I can exit the REPL by pressing **CTRL+D** or **CTRL+C** twice.

## 4. Differences Between Node.js and Browser JavaScript

### Execution Environment:

- **Node.js** runs on the server-side and executes JavaScript outside the browser environment. It’s used to build server applications.
- **Browser JavaScript** runs in the browser and interacts with the DOM (Document Object Model) to manipulate web pages, handle events, etc.

### Global Objects:

- In **Node.js**, I have access to global objects like `__dirname`, `process`, `require`, etc., which are not available in the browser environment.
- In the **browser**, I can interact with objects like `window`, `document`, and `localStorage`.

### Asynchronous Nature:

- **Node.js** is event-driven and non-blocking. It uses asynchronous I/O operations, meaning it doesn’t wait for a task to finish before moving on to the next. For example, if reading a file takes time, Node.js doesn’t block the process; it moves on to other tasks while waiting for the file to finish loading.
- **Browser JavaScript**, on the other hand, often deals with the event loop and asynchronous code via callbacks or Promises, but it’s primarily concerned with user interface interactions.

### Why Node.js is Suitable for Servers:

- **Concurrency**: Node.js can handle many requests simultaneously without creating a new thread for each request, thanks to its event loop. This makes it lightweight and ideal for building scalable applications.
- **Real-time Applications**: Node.js is excellent for real-time apps because it allows for constant communication between the client and server without needing to refresh the page, which is commonly used in chat apps, online gaming, and collaborative tools.

## 5. My first Node.js Script. Yay!

- As I have covered the basics it is now time to get my hands dirty and create a script which strores the code in a file instead of executing immediately like the REPL does.

  - A script called `app.js` will be populated with this content:
    ```javascript
    console.log("Yay! My first Node.js script");
    ```
  - To run the code I simply run this on the terminal:
    ```bash
    node app.js
    ```

## **Resources I’m Using**

- [Node.js Official Documentation](https://nodejs.org/en/docs/)
- [Node.js Guide for Beginners](https://nodejs.dev/)
- [Understanding Event Loop](https://developer.mozilla.org/en-US/docs/Web/JavaScript/EventLoop)
