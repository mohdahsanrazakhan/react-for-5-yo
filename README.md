# ⚛️ ReactJS for 5 y/o 🧒

## What is React?

- React is an open-source JavaScript library for building user interfaces for web applications
- Developed and maintained by Facebook (now Meta)
- React is widely used to create interactive and dynamic web applications

### Here's a simplified breakdown: (optional)

- **Open-source** refers to software or projects where the original creators provide the underlying _code and resources for anyone to view, use, modify, and share freely_.<br>
  It's like sharing a recipe for a dish you've created, allowing others to see how it's made, make improvements, and share their versions without any restrictions. Open-source fosters collaboration and innovation by making knowledge and tools accessible to a wide community of people.

- **JavaScript library** is like a _collection of pre-written code_ that helps web developers do common tasks more easily and quickly when building websites or web applications.<br>
  It's like having a toolbox full of tools that you can use instead of having to create each tool from scratch.<br>
  These libraries provide ready-made functions and features, saving time and effort in coding, and making it easier to create interactive and dynamic websites.

- **User Interface (UI)** is like the _"face" of a computer program or a digital device_. It's what you see and interact with on your screen when you use software or apps.<br>
  UI design focuses on making this interaction as user-friendly and easy to understand as possible. It includes things like buttons, menus, icons, and how information is displayed, all aimed at making your experience pleasant and efficient when using technology.<br>
  Essentially, it's the bridge that allows you to communicate and control the digital world with your clicks, taps, and gestures.

- **Web Application** is like a _software program that you can use through a web browser_, just like how you use websites. It's a tool or service that helps you do things on the internet, like checking your email, shopping online, or using social media.<br>
  Unlike regular websites that mostly provide information, web applications allow you to interact with them, input data, and get specific results or perform tasks online, making them more like digital tools than just pages to read.

## React Installation

### Prerequisites:

Node.js: Ensure you have Node.js installed on your system. To check the version of Node.js run `node -v` or `node --version` and `npm -v` or `npm --version`. Don't worry about NPM, it installed with node.<br>
If you don't download it yet. Go to the [official Node.js website](https://nodejs.org/en/download).

### Commands for installing ReactJS using CRA:

Navigate to the directory where you want to create your React project. <br>
**Run the following command to create a new React application using Create React App (CRA):**

```bash
npx create-react-app my-react-app
```

Replace my-react-app with your desired project name.<br>
**Run the following command to navigate to the project directory:**

```bash
cd my-react-app
```

**Once you're inside the project directory, you can start the development server by running:**

```bash
npm start
```

or

```bash
npm run start
```

> **_Want to install React faster than above?_**

### Commands for installing ReactJS using Vite:

**Run the following command to create a new React application using Vite:**

```bash
npm create vite@latest my-react-app -- --template react
```

Replace my-react-app with your desired project name.
**After the project is created, navigate to your project directory using the cd command:**

```bash
cd my-react-app
```

**Run the following command to install the project dependencies:**

```bash
npm install
```

**After the dependencies are installed, you can start the development server by running:**

```bash
npm run dev
```

## What is a React Components

A React component is _a reusable, self-contained building block_ of a user interface in a React application. It represents _a part of the UI that can have its own logic, state, and rendering behavior_.<br>
React components are at the core of building web interfaces with React, and they can range from simple, isolated elements like buttons or form inputs to complex, nested structures like entire sections of a webpage.

### Here's a simplified breakdown: (optional)

- **Rendering:** refers to _the process of turning your React components into a user interface (UI)_ that users can see and interact with on a web page. It's like taking the blueprint (your React components) and actually building the house (the visible and interactive part of your website) based on that blueprint.<br>
  When you write React code, you create components that describe what your UI should look like and how it should behave. React then takes these components and renders them onto the web page, making them visible to users. This _rendering process involves updating the UI whenever there are changes in your data or when user interactions occur_.<br>
  So, rendering in React is _all about making your web application come to life by taking your code and displaying it_ as a functional and interactive user interface.
- **Reusability:** React components are designed to be reusable. You can _create a component once and use it multiple times across your application_. This promotes a modular and efficient approach to UI development.
- **State:** Components can have their own state, which is a data store that can change over time. When the state of a component changes, React automatically re-renders the component to reflect those changes in the UI.

## What is a React JSX

JSX, which stands for **JavaScript XML**, is _a syntax extension for JavaScript_ often used with React. JSX _allows you to write HTML-like code within your JavaScript code_, making it easier to describe the structure and content of your user interfaces.

### Key features of JSX include:

- **HTML-Like Syntax:** JSX looks similar to HTML. You can use tags like `<div>`, `<p>`, and `<h1>` to define elements in your components.
- **Embedding Expressions:** can _embed JavaScript expressions within JSX using curly braces {}_. This allows you to include _dynamic data or logic directly_ in your JSX code.
- **Components:** JSX also _allows you to use React components just like HTML elements_. For example, if you have a custom Button component, you can use it in JSX as `<Button />`.

**Here's an example of JSX in a React component:**

```javascript
import React from "react";

function MyComponent(props) {
  const greeting = "Hello, React JSX!";
  return (
    <div>
      <h1>{greeting}</h1>
      <p>This is an example of JSX in a React component.</p>
    </div>
  );
}

export default MyComponent;
```

In this example:

`<div>`, `<h1>`, and `<p>` are JSX elements representing HTML tags.<br>
{greeting} is a JavaScript expression embedded within JSX, and it will be replaced with the value of the greeting variable.<br>
MyComponent is a React functional component.<br>
JSX is transpiled (converted) into regular JavaScript code by build tools like Babel before it's executed in the browser. This transpilation step is necessary because browsers don't understand JSX directly. The transformed JavaScript code is what actually creates and updates the DOM elements when the component is rendered.<br>

Overall, JSX simplifies the process of creating and maintaining React components by allowing you to express UI structures in a familiar, HTML-like syntax while still leveraging the power of JavaScript.
