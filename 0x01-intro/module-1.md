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

- **Exiting the REPL**: I can exit the REPL by pressing **CCTRL+D** or **CTRL+C** twice.
