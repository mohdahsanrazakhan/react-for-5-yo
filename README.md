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

Replace `my-react-app` with your desired project name.<br>
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

Replace `my-react-app` with your desired project name.
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

### Here are key characteristics and concepts related to React components:

- **Reusability:** React _components are designed to be reusable_. You can create a component once and use it multiple times across your application. This promotes a modular and efficient approach to UI development.

- **Encapsulation:** Components _encapsulate both the UI and the logic related to that UI_. This encapsulation keeps the code _organized and maintains a separation of concerns_.

- **State:** Components can have their own _state_, which is a _data store that can change over time_. When the state of a component changes, React automatically re-renders the component to reflect those changes in the UI.

- **Props (Properties):** _Components can receive data from their parent components through props_. Props are like parameters that allow you to customize the behavior and appearance of a component when you use it in different contexts.

- **Lifecycle Methods:** Components have a lifecycle, which consists of various methods that are automatically invoked at different stages of a component's existence. These methods allow you to perform actions such as initializing state, making API requests, or cleaning up resources.

- **Rendering:** refers to _the process of turning your React components into a user interface (UI)_ that users can see and interact with on a web page. It's like taking the blueprint (your React components) and actually building the house (the visible and interactive part of your website) based on that blueprint.<br>
  When you write React code, you create components that describe what your UI should look like and how it should behave. React then takes these components and renders them onto the web page, making them visible to users. This _rendering process involves updating the UI whenever there are changes in your data or when user interactions occur_.<br>
  So, rendering in React is _all about making your web application come to life by taking your code and displaying it_ as a functional and interactive user interface.

- **Hierarchy:** React components can be _organized into a hierarchy or tree structure, with parent components containing child components_. Changes to a parent component can affect its children, allowing for complex, interactive UIs.

- **Functional and Class Components:** React components can be _defined using either JavaScript classes (class components)_ or _JavaScript functions (functional components)_. Functional components are becoming more common, especially with the introduction of React Hooks.

- **Component Composition:** You can _compose more complex UIs by combining multiple smaller components_. This promotes code reusability and maintainability.

- **Custom Components:** In addition to using built-in HTML elements like `div` and `span`, you can create custom components to represent parts of your UI that have specific functionality or styling.

## What is a React JSX

JSX, which stands for **JavaScript XML**, is _a syntax extension for JavaScript_ often used with React. JSX _allows you to write HTML-like code within your JavaScript code_, making it easier to describe the structure and content of your user interfaces.

### Key features of JSX include:

- **HTML-Like Syntax:** JSX looks similar to HTML. You can use tags like `<div>`, `<p>`, and `<h1>` to define elements in your components.
- **Embedding Expressions:** can _embed JavaScript expressions within JSX using curly braces `{}`_. This allows you to include _dynamic data or logic directly_ in your JSX code.
- **Components:** JSX also _allows you to use React components just like HTML elements_. For example, if you have a custom `Button` component, you can use it in JSX as `<Button />`.

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
`{greeting}` is a JavaScript expression embedded within JSX, and it will be replaced with the value of the `greeting` variable.<br>
`MyComponent` is a React functional component.<br>
JSX is transpiled (converted) into regular JavaScript code by build tools like Babel before it's executed in the browser. This transpilation step is necessary because browsers don't understand JSX directly. The transformed JavaScript code is what actually creates and updates the DOM elements when the component is rendered.<br>

Overall, JSX simplifies the process of creating and maintaining React components by allowing you to express UI structures in a familiar, HTML-like syntax while still leveraging the power of JavaScript.

## What is a React Props

In React, **props** is short for _properties_, and _it refers to a mechanism for passing data from a parent component to a child component_. Props are a fundamental part of React's component architecture and are _used to make components dynamic and reusable_.

### Here are the key points to understand about React props:

- **Passing Data:** Props allow you to pass data (values or objects) from a parent component to a child component. This data can be used by the child component to customize its behavior or render dynamic content.

- **Immutable:** _Props are immutable_, which **means** that the _child component receiving props cannot modify them_. They are _read-only, ensuring that data flows in one direction, from parent to child_.

- **Functional and Class Components:** Props can be used with both functional components (using function arguments) and class components (accessed via this.props).

- **Accessing Props:** In a **functional component**, you can _access props as arguments to the component function_. In a **class component**, you _access props using `this.props`_.

- **Default Values:** You can specify default values for props, which will be used if the parent component doesn't provide a value for a particular prop.

- **Dynamic Rendering:** Props enable dynamic rendering by allowing you to conditionally render content based on the values of props.

Here's a simple example of how props work in React:

```javascript
// ParentComponent.js
import React from "react";
import ChildComponent from "./ChildComponent";

function ParentComponent() {
  const name = "Alice";

  return (
    <>
      <h1>Parent Component</h1>
      <ChildComponent name={name} />
    </>
  );
}

export default ParentComponent;
```

```javascript
// ChildComponent.js
import React from "react";

function ChildComponent(props) {
  return <p>Hello, {props.name}!</p>;
}

export default ChildComponent;
```

In this example:

- `name` is a prop passed from ParentComponent to ChildComponent.
- In ChildComponent, `{props.name}` is used to access and render the value of the name prop.

By using props, you can _create reusable components_ that can be configured differently when used in various parts of your application. _Props are essential for building dynamic and data-driven user interfaces in React_.

## What is React State

In React, **state** is a _JavaScript object_ used _to store and manage data that can change over time and affect a component's behavior and rendering_. Each React component can have its own state, which is used to keep track of information that should be reactive to user interactions, data fetching, or other dynamic changes.

### Key points about React state:

- **Component-Specific:** _State is local to a component_. Each instance of a component maintains its own state, making it independent of other instances of the same component.

- **Initialization:** State is typically _initialized in a component's constructor or by using a React Hook (in functional components)_. For **class components**, you _set the initial state using `this.state` in the constructor_. In **functional components**, you use the _useState Hook to initialize state_.

- **Updating State:** State can be _updated using the setState method_ in class components or by calling the state updater function returned by the useState Hook in functional components. _React automatically re-renders the component when state is updated_.

- **Immutable:** State should be treated as immutable. You should _not directly modify state_; instead, _use setState (for class components)_ or provide a _new state object (for functional components)_ when updating state.

- **Asynchronous Updates:** State updates are asynchronous in React. This means that _React batches multiple state updates together for performance reasons_. If you need to perform actions after a state update, _use a callback function provided to setState or the useState Hook_.

- **Local Scope:** State is _accessible only within the component where it is defined_. It cannot be directly accessed or modified by parent or sibling components. _If you need to share state between components, you can lift the state up to a **common ancestor component** and pass it down as props_.

**Rendering Based on State:** React components typically render based on the values stored in their state. _When state changes, the component automatically re-renders to reflect those changes in the user interface_.

Here's a simple example of how state is used in a React **class component**:

```javascript
import React, { Component } from "react";

class Counter extends Component {
  constructor(props) {
    super(props);
    this.state = {
      count: 0,
    };
  }

  incrementCount = () => {
    this.setState({ count: this.state.count + 1 });
  };

  render() {
    return (
      <div>
        <p>Count: {this.state.count}</p>
        <button onClick={this.incrementCount}>Increment</button>
      </div>
    );
  }
}

export default Counter;
```

In this example, the `count` variable is stored in the component's state. When the **Increment** button is clicked, the `incrementCount` method is called, which updates the `count` state, causing the component to re-render with the new count value. State allows you to create interactive and dynamic user interfaces in React applications.

Certainly! Here's the same counter example using a **functional component** and the _useState Hook_ in React:

```javascript
import React, { useState } from "react";

function Counter() {
  const [count, setCount] = useState(0);

  const incrementCount = () => {
    setCount(count + 1);
  };

  return (
    <div>
      <p>Count: {count}</p>
      <button onClick={incrementCount}>Increment</button>
    </div>
  );
}

export default Counter;
```

In this functional component:

- We import `useState` from the **\*react** library\* to manage the component's state.
- Inside the `Counter` component, we use the `useState` Hook to declare the `count` state variable and its corresponding updater function, `setCount`. We initialize `count` to `0`.
- When the **Increment** button is clicked, the `incrementCount` function is called, which updates the `count` state using `setCount`, just like `setState` in class components.
- The component renders the `count` value and the **Increment** button, and it automatically re-renders whenever `count` changes.

Functional components with Hooks offer a more concise and modern way to manage state in React applications.

## What is a React Events

In React, events refer to actions or interactions that occur in the user interface, such as clicking a button, typing in an input field, or moving the mouse. React allows you to handle these events by attaching event listeners to elements in your components, just like you would in traditional web development.

### Here are the key points to understand about React events:

- **Event Handling:** React components can _define event handlers_, which _are JavaScript functions that get executed in response to specific events_. For example, you can define an `onClick` event handler to handle a button click.

- **Event Attributes:** In JSX, you can _attach event handlers to elements using special attributes named after the event_, such as `onClick`, `onMouseOver`, `onChange`, etc. These attributes take a _reference to a function that will be called when the event occurs_.

- **Event Object:** React passes an event object as the first argument to event handler functions. This _object contains information about the event_, such as the _target element, mouse coordinates, key codes, and more_.

- **Binding Event Handlers:** When defining event handlers in **class components**, you often _need to manually bind them to the component instance using `.bind()` or arrow functions_. In **functional components**, this is _not necessary when using the function syntax_.

- **Event Propagation:** React follows the same event propagation model as the browser's native events. Events bubble up from child to parent components, and you can stop propagation or prevent the default behavior of events as needed.

- **Synthetic Events:** React provides a _synthetic event system that normalizes browser-specific event behavior_, ensuring consistent behavior across different browsers.

Here's an example of handling a click event in a React component:

```javascript
import React from "react";

function MyComponent() {
  const handleClick = (event) => {
    alert("Button clicked!");
    // You can access event properties like event.target, event.clientX, etc.
  };

  return (
    <div>
      <button onClick={handleClick}>Click me</button>
    </div>
  );
}

export default MyComponent;
```

In this example:

- We define a `handleClick` function to be executed when the button is clicked.
- We attach the `handleClick` function to the button's `onClick` event attribute.
  When the button is clicked, the `handleClick` function is called, and it shows an alert.

React events provide a way to create interactive and responsive user interfaces by allowing you to respond to user interactions with your application.
