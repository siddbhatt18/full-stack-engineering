# Full Stack Engineering Roadmap 2026
### Complete Web Dev + GenAI + DevOps + System Design + Projects

---

## Phase 1 — Fundamentals (Internet, Tools & Environment)

### 1. How the Internet Works
- History of Web (Web 1.0 to Web 3.0)
- How computers communicate with each other
- How computers send data all over the world
- What is Domain Name, IP & MAC Addresses and Routing
- How ISP and DNS work together to deliver data

### 2. Client-Server Architecture
- What is Client-Server Model
- Difference between Client (browser) and Server
- How HTTP request and response cycle works
- What happens when you visit a website
- Difference between Front-end and Back-end
- What are Static Websites and Dynamic Websites
- What is web hosting and how it works

### 3. Internet Protocols
- What is TCP protocol and why it is widely used
- How Connection is established using TCP (3-Way Handshake)
- What is UDP and why it's used for fast communication
- How UDP establishes connection
- Difference between TCP and UDP

### 4. Understanding HTTP & HTTPS
- What is HTTP and its different versions
- HTTP status codes for responses
- What is HTTPS and why it's better than HTTP
- How HTTPS provides a secure connection
- What is SSL/TLS Encryption
- What are Proxy and Reverse Proxy
- How VPN works and helps accessing restricted content

### 5. Preparing Your Machine
- Installing & Setting up VS Code
- Installing helpful extensions
- Setting up your browser for development
- What are files and folders and how to create them
- Testing environment via serving a webpage — "Namaste Duniya"
- Learning basic terminal commands — `pwd`, `ls`, `cd`, `mkdir`, `clear`

---

## Phase 2 — HTML

### 6. Starting with HTML
- Understanding HTML and its use cases
- Creating first HTML page in VS Code
- Understand HTML Structure
- Understanding Tags and building simple HTML page — `doctype`, `html`, `head`, `title`, `body`
- Working with text elements — `h` tags, `p`, `br`, `a`, `span`, `code`, `pre`
- Working with HTML Lists (Ordered & Unordered) — `ol`, `ul`, `li`
- Understanding nested elements in HTML
- Working with Media Tags — `img`, `video`, `audio`
- HTML attributes — `href`, `target`, `alt`, `src`, `width`, `height`
- Navigating between pages

### 7. More on HTML
- Understanding semantic tags — `article`, `section`, `main`, `aside`, `form`, `footer`, `header`, `details`, `figure`
- Differentiating between block and inline elements
- Text formatting tags — `b`, `strong`, `i`, `small`, `ins`, `sub`, `sup`, `del`, `mark`
- Working with HTML tables — `table`, `td`, `tr`, `th`

### 8. Semantic HTML & Browser Rendering
- How Browsers Render Pages — HTML parsing → CSSOM → Render Tree → Paint
- Understanding Reflow & Repaint — Why layout shifts happen
- SEO Impact of Semantic HTML — Why structure improves search ranking
- Accessibility Basics — Intro to ARIA roles and inclusive design
- Content Structure — Headings hierarchy for clean document flow
- Responsive Images — Basic introduction to image optimization
- Links & Navigation Flow — Internal vs external linking strategies

### 9. HTML Forms and Inputs
- What is Form and why it's important
- Creating a simple Form — `form`, `input`, `textarea`, `select`, `button`, `label`
- Types of input fields — `checkbox`, `text`, `color`, `file`, `tel`, `date`, `number`, `radio`, `submit`, `range`
- Attributes of Form Elements — `method`, `action`, `target`, `novalidate`, `enctype`, `name`, `required`, `placeholder`
- Forms Introduction — Structure of form, input types, validation basics

### 10. Media Tags in HTML
- Understanding `audio` and `video` tags
- Attributes of media tags — `src`, `width`, `height`, `alt`, `muted`, `loop`, `autoplay`, `controls`, `media`
- Using `source` element for alternative media files

---

## Phase 3 — CSS

### 11. Basics of CSS (Cascading Style Sheet)
- Introduction to CSS and why it is important
- Understanding Syntax, Selectors and comments in CSS
- Adding CSS to HTML Page — Inline, Internal, External
- CSS Syntax & Selectors — Element, class, id, grouping selectors, parent selector
- Understanding precedence/specificity of selectors
- Specificity & Cascade — Why some styles override others
- Inheritance & Computed Styles — How CSS flows across elements
- How to style text using CSS — font family, font style, font weight, line-height, text-decoration, text-align, text-transform, letter-spacing, word-spacing, text-shadow

### 12. Styling with CSS
- Working with colors in CSS — name, rgb, hex, hsl, etc.
- Working with CSS units — `%`, `px`, `rem`, `em`, `vw`, `vh`, `min`, `max`
- Working with borders and border styling
- Box Model Deep Understanding — Content, padding, border, margin, box-sizing, height, width
- Understanding Background properties — background-size, background-attachment, background-image, background-repeat, background-position, linear-gradient
- Implementing shadow property
- Modern CSS Functions — `clamp()`, `min()`, `max()` for fluid design
- CSS Variables — Using `:root` for global theming
- Design System & Design Tokens Concept — Building reusable spacing & color systems

### 13. CSS Layout Mastery
- Display properties — `inline`, `grid`, `flex`, `none`, `inline-block`, etc.
- Flexbox Deep Dive — Axis control, alignment, distribution mastery, `flex-direction`, `order`, `flex-wrap`, `flex-grow`, `flex-shrink`, `justify-content`, `align-items`, `align-content`, `align-self`, `flex-basis`, shorthand properties
- Common Layout Patterns — Navbar, card grid, center alignment tricks
- CSS Grid — Grid template areas & 2D layout control
- Combining Grid & Flex — Real-world layout architecture
- Positioning — `relative`, `absolute`, `fixed`, `sticky`, `static` with practical examples
- Stacking Context — Understanding `z-index` properly
- Container Queries — Modern responsive component design
- Understanding Overflow — `visible`, `hidden`, `scroll`
- Grouping Selectors and Nested Selectors

### 14. CSS Animations & Motion Design
- Pseudo classes and Pseudo Elements — `hover`, `focus`, `after`, `before`, `active`
- CSS Transitions — Timing functions, duration, properties, delays
- Transform — `translate`, `scale`, `rotate`, `skew` for interactive UI
- 3D Transforms — `translate3d()`, `translateZ()`, `scale3d()`, `scaleZ()`, `rotate3d()`, `rotateZ()`
- Keyframe Animations — `@keyframes`, creating smooth motion systems
- Performance Considerations — When NOT to animate

### 15. CSS Responsive Design
- Difference between Mobile-First and Desktop-First
- Media Queries — `@media`, `max-width`, `min-width`
- Breakpoint Planning — Structured scaling approach
- Viewport meta element for Responsive
- Responsive Images — `object-fit`, performance awareness
- Fluid Typography — `clamp()` for dynamic text sizing
- Spacing Rhythm — Consistent vertical and horizontal spacing systems
- Measurement units for Responsive Design — `px`, `in`, `mm`, `%`, `rem`

### 16. CSS Architecture & Project Structure
- BEM Naming Convention — Avoiding messy class systems
- Component-Based CSS — Designing reusable style blocks
- Utility Classes vs Component Classes — Pros & cons
- Real-World Folder Structure — `css/`, `components/`, `layout/`, `utilities/`
- Debugging with DevTools — Inspecting overflow & layout shifts

### 17. Working with SASS (SCSS)
- What is SASS? Variables, Nesting, Mixins, Functions and Operators
- Setting up environment for SCSS
- SCSS or SASS? and Setting Up SCSS
- Working with SASS — Variables, Nesting, Partials and Imports, Mixins, Inheritance/Extends, Functions, Operators
- Advanced Concepts — Control Directives, Color Functions

### 18. CSS Frameworks — TailwindCSS & Bootstrap
- Introduction to CSS frameworks and their role in modern frontend development
- Understanding utility-first vs component-based styling approaches
- Overview of TailwindCSS and why it is popular
- Setting up TailwindCSS in a project
- Working with Tailwind utility classes for layout, spacing, colors, and typography
- Building responsive layouts using TailwindCSS
- Introduction to Bootstrap and its component-based design system
- Using the Bootstrap grid system for responsive layouts
- Working with common Bootstrap components — navbar, cards, buttons
- Customizing Bootstrap styles for real-world projects
- Comparing TailwindCSS and Bootstrap — when to use which

---

## Phase 4 — JavaScript

### 19. Introduction to JavaScript
- What is JavaScript & Why It Powers the Web
- Where JavaScript Runs — Browser & Node.js overview
- Linking JS with HTML using `script` tag
- Running JavaScript in the Browser Console
- Using Console for Debugging & Testing — `console.log()`, `console.info()`, `console.warn()`, `prompt`, `alert`
- Variables — `var`, `let`, `const` with scope understanding
- Naming Conventions & Clean Code Practices
- Data Types — `number`, `float`, `string`, `boolean`, `null`, `undefined`, `array`, `object`, `Symbol` (Primitive & Non-Primitive)
- Some Important Values — `undefined`, `null`, `NaN`, `Infinity`
- Working with Strings — `splice`, `slice`, `template string`, `split`, `replace`, `includes`
- What are Statements, Semicolons, Expressions (difference between expression and statement)
- How to add Comments in JavaScript
- Mini Practice Programs — Calculator, Greeting system, Input handling via prompt
- Variable hoisting in JavaScript

### 20. Operators & Type System
- Arithmetic Operators — `+`, `-`, `*`, `/`, `%`, `++`, `--`
- Comparison Operators — `==` vs `===`, `!=`
- Logical Operators — AND, OR, NOT usage patterns
- Assignment Operators — Practical usage
- Bitwise Operators
- `typeof` Operator — Identifying data types dynamically
- Truthy & Falsy Values — Real-world conditional traps
- Type Coercion — Implicit vs explicit conversion

### 21. Conditionals & Loops
- `if`, `else-if`, `else` branching logic
- Ternary Operator
- `switch` statement for structured decision-making
- `for` loop iteration patterns
- `while` & `do-while` usage cases
- `forEach` in JavaScript
- `for...in` Loop in JavaScript
- `for...of` Loop in JavaScript
- `break` & `continue` control flow statements
- Recursion in JavaScript
- Practice — Prime number check, multiplication table, pattern printing

### 22. Functions
- Function Declaration vs Function Expression
- Parameters & Arguments deeply explained — required, destructured, rest, default
- Arguments — positional, default, spread
- Return Values & Scope
- Arrow Functions (ES6+)
- Classic Function, Nested Function (function within function), Scope Chain
- Immediately Invoked Function Expression (IIFE)
- More Functions — Arrow Function, Fat Arrow, Anonymous, Higher Order, Callback, First Class, Pure Function, Impure Function
- Writing Reusable Logic Blocks
- Understanding Scoping — Global scope, Function scope
- Understanding Closures, Scoping Rule
- Recursion
- Practice — Grade calculator, even/odd checker, reusable utility functions

### 23. Arrays
- Creating Arrays — What arrays are and when to use them
- Accessing Elements — Indexing basics
- Array Operations — `push`, `pop`, `shift`, `unshift`
- `length` Property — Counting items in an array
- `indexOf`, array destructuring
- Basic Iteration — Looping with `for` / `while` / `forEach`
- Multidimensional Arrays
- Practice — Todo list in array, max/min finder

### 24. Array Methods
- `map()` — Transforming arrays
- `filter()` — Selecting items based on conditions
- `reduce()` — Accumulating values into a single output
- `forEach()` — Iteration without returning a new array
- `some()` / `every()` — Boolean checks on arrays
- `slice()` / `splice()` — Copying vs modifying arrays
- `sort()` — Sorts the array in place and returns it
- `flat()` — Flattens nested arrays into one level
- `reverse()`, `join()`, `toString()`
- Spread operator
- Introduce functional thinking lightly
- Practice — Filter students by marks, transform user list, calculate total price

### 25. Objects
- What is an Object? — Real-world modeling with key-value data
- Key-Value Pairs — Understanding properties and values
- Accessing Properties — Dot notation vs bracket notation
- Adding / Deleting Properties — Mutating objects safely
- Nested Objects — Deep data structures
- Looping Through Keys — `for...in` and `Object.keys()`
- How Objects Are Stored, Traverse Keys, Array as Object
- Timing Events — `setTimeout()`, `setInterval()`, `clearTimeout()`, `clearInterval()`
- Practice — User profile system, cart object

### 26. Object Methods
- `Object.entries()` — Converts an object into an array of [key, value] pairs
- `Object.assign()` — Copies properties from source objects
- `Object.freeze()` — Makes an object immutable
- `Object.seal()` — Prevents adding or deleting properties
- `Object.fromEntries()` — Converts array of [key, value] pairs back into object
- `Object.is()` — Edge-case safe equality comparison
- `Object.keys()` — Returns array of all keys
- `Object.values()` — Returns array of all values
- Object destructuring, object methods, `this` keyword

### 27. Document Object Model (DOM) Manipulation
- Introduction to DOM in JavaScript
- Understanding DOM Structure and Tree — nodes, elements, document
- Fetching Elements — `getElementById`, `getElementsByTagName`, `getElementsByClassName`, `querySelectorAll`, `querySelector`
- DOM Tree Traversal — `parentNode`, `childNodes`, `firstChild`, `nextSibling`
- Manipulating DOM Elements — `innerHTML`, `textContent`, `setAttribute`, `getAttribute`, `style` property, `classList`
- Creating and Removing DOM Elements — `createElement()`, `appendChild()`, `insertBefore()`, `removeChild()`

### 28. Event Handling in JavaScript
- Event Handling — `addEventListener()`, event bubbling, `event.target`
- Scroll Events, Mouse Events, Key Events and Strict Mode
- Working with Forms and Input Elements — Accessing Form Data, Validating Forms, `preventDefault()`, `onsubmit`, `onchange`
- Working with Classes — Adding, Removing, Toggling (`classList` methods)
- Browser Events — `DOMContentLoaded`, `load`, `resize`, `scroll`

### 29. Using Browser Functionalities in JavaScript
- Browser Object Model — `window`, `navigator`, `history`, `location`, `document`
- Window Object — `window.location`, `window.history`
- Working with Storage — Local Storage, Session Storage, Cookies
- Web APIs in DOM — Fetch API

### 30. Object Oriented Concepts in JavaScript
- Introduction to OOP in JavaScript
- Understanding classes and objects in JavaScript
- Understanding Constructor and Prototypes — `this` keyword, `call`, `apply`, `bind`
- Class expression, hoisting, inheritance, getter & setter

### 31. Asynchronous Programming in JavaScript
- Introduction to Asynchrony in JavaScript
- Introduction to callbacks and Problems in Callbacks (Callback Hell)
- Understanding promises — `pending`, `resolved`, `rejected`
- How to prevent callback hell using `async` & `await`
- `setInterval` & `setTimeout` in JavaScript

### 32. Error Handling in JavaScript
- Introduction to Error Handling
- Common types of errors — Syntax errors, Runtime errors, Logical errors
- Understanding the Error object — `message`, `name`, `stack`
- Handling exceptions using `try-catch`, `try-catch-finally`
- How to Throw Errors in JavaScript
- How to create custom errors in JavaScript
- Error Handling in Asynchronous Code

### 33. Advanced JavaScript Topics
- Throttling and Debouncing uses in JavaScript
- JSON Handling — `JSON.parse()`, `JSON.stringify()`

### 34. Git and GitHub
- What is Git and GitHub?
- Concepts — Git commits, Understanding branches, Making branches, Merging branches, Conflict resolution, Understanding workflow, Pushing to GitHub
- How to use GitHub with team members, forking, PR (pull requests), open source contribution, workflow with large teams

---

## Phase 5 — TypeScript

### 35. TypeScript Essentials
- What is TypeScript and why it exists
- Thinking in TypeScript — Types-first mindset
- Installing and Setting Up TypeScript
- Introduction to `tsconfig.json`
- Understanding compiler options and strictness levels
- TypeScript Compiler (`tsc`)
- Target environments and module systems
- Integrating TypeScript with modern build tools
- Linting and Formatting with TypeScript

### 36. TypeScript Basic Types & Data Structures
- Understanding TypeScript type system
- Basic/Primitive Types — `string`, `number`, `boolean`, `any`, `unknown`
- Difference between `any`, `unknown`, `never`, and `void`
- Nullable types and undefined handling
- Arrays and typed collections
- Tuples and fixed-length data structures
- Read-only types and immutability concepts

### 37. Object Typing in TypeScript
- Typing objects in TypeScript
- Required vs optional properties
- Read-only properties
- Nested object typing
- Index signatures
- Excess property checks
- Structural typing concept

### 38. Advanced Type Definitions
- Type aliases and their purpose
- Interfaces vs Type Aliases — When to use what
- Union and Intersection Types — Modeling flexible data
- Literal types and value constraints
- Optional chaining and null safety concepts
- Type narrowing and control flow analysis

### 39. Interfaces in TypeScript
- Introduction to interfaces
- Defining object contracts using interfaces
- Interface extension and inheritance
- Declaration merging
- Interfaces vs type aliases
- Best practices for using interfaces in React projects

### 40. Enums and Constants Management
- Introduction to enums
- Numeric vs string enums
- Use cases for enums in frontend applications
- Alternatives to enums
- Managing constants in TypeScript projects

### 41. Generics in TypeScript
- Understanding generic types
- Why generics are important
- Generic Functions — Reusable logic with type safety
- Generic Interfaces and Constraints — Safe boundaries
- Practical use cases of generics in React applications

### 42. TypeScript Best Practices & Debugging
- Understanding strict mode in TypeScript
- Benefits of strict type checking
- Avoiding misuse of `any`
- Writing clean and predictable type definitions
- Type reuse and centralization strategies
- Understanding TypeScript compiler errors
- Debugging type mismatches
- Handling null and undefined safely
- Working with third-party library typings

---

## Phase 6 — React & Frontend Architecture

### 43. Introduction to React
- Why React Exists — Problems with manual DOM manipulation
- What is React, and Why Use It?
- Declarative vs Imperative UI
- What is SPA (Single Page Application) — SPA vs Multi-Page Applications
- Real DOM vs Virtual DOM — How React optimizes rendering performance
- What are Components and types — class component, function components
- Setting Up React with Vite — Installing project, folder understanding
- Project Structure Breakdown — `src`, `components`, `assets`, `public` folder
- JSX Syntax Rules — Embedding JavaScript inside HTML-like syntax, Fragments, Components Naming
- Component-Based Architecture — Breaking UI into reusable logical units
- NPM Basics | Installing Packages
- How updates work in React, ES6+ features like Import & Exports
- Difference Between React and Other Frameworks (Angular, Vue)
- Installing React Developer Tools

### 44. Styling in React
- Different Styling Approaches
- Importance of component-based styling — Inline Styles, CSS Modules
- Importing CSS file/stylesheet in React
- Adding a CSS Modules Stylesheet — Styled Components, Dynamic styling with styled-components
- Dynamic Styling Based on Props or State
- Responsive Design in React
- Media queries with CSS and styled-components

### 45. React Components & Props
- Functional Components — Writing reusable UI functions
- Understanding Props — Passing data between components
- Dynamic Rendering — Rendering UI based on props data
- Rendering Lists — Using `map()` to generate repeated UI blocks
- Keys in React — Why unique keys are critical for performance
- Creating Reusable Card Component
- Creating Parameterised Function Components

### 46. State & Re-rendering Logic
- What is State? — Data that changes over time
- `useState` Hook — Managing local component state
- Creating a state and Managing State using `setState`
- How React Re-renders — Understanding reconciliation process
- Batching State Updates — Performance optimization internally
- Derived State Concept — Avoiding unnecessary state variables
- Practical Build — Interactive counter, toggle switch UI

### 47. React Lifecycle Methods
- Class Components Lifecycle — Component lifecycle flow
- React's Lifecycle Methods — `componentDidMount`, `componentDidUpdate`, `componentWillUnmount`
- `useEffect` Hook — Side effects in functional components
- Data Fetching, Cleanup & DOM Manipulation — Practical patterns and best practices
- Mounting, Updating, Unmounting

### 48. Event Handling & Conditional Rendering
- Handling Click Events in React
- Controlled Inputs — Managing form inputs via state
- Conditional Rendering Patterns — `&&` operator, ternary operator, early return
- Dynamic UI Rendering — Showing/hiding components
- Function chaining in React — Rendering Array Data via `map`, Eliminating via `filter`
- Practical Build — Dynamic form with validation logic

### 49. Component Architecture Principles
- Single Responsibility Principle — One component, one responsibility
- Smart vs Dumb Components — Separation of concerns in UI
- Lifting State Up — Sharing data between sibling components
- Prop Drilling Problem — Why deep passing becomes messy
- Component Composition — Building scalable layout systems

### 50. Useful Hooks in React
- Understanding React Hooks
- Rules of hooks
- Commonly Used Hooks: `useState`, `useEffect`, `useContext`, `useRef`, `useCallback`, `useMemo`
- Custom Hooks — When and How to Create Them
- Understanding and Applying Context API

### 51. useEffect Deep Dive
- What `useEffect` Really Does — Synchronizing with external systems
- Dependency Array Behavior — Why infinite loops happen
- Cleanup Functions — Preventing memory leaks
- Data Fetching Pattern with `useEffect`
- Practical Example — Fetching API data on component mount

### 52. Custom Hooks & Reusable Logic
- Why Custom Hooks Exist — Extracting shared logic
- Writing a `useFetch` Hook — Reusable API fetching logic
- Separation of Business Logic from UI
- Improving Code Maintainability with Hooks

### 53. Advanced Reusability Patterns
- Higher Order Components (HOCs) — Reusing behavior by wrapping components
- Render Props Pattern — Sharing logic through a function prop
- Compound Components — Designing flexible component APIs with shared internal state

### 54. Routing & Application Structure
- Introduction to React Router — Client-side navigation system
- Setting Up and Configuring React Router (`react-router-dom`)
- Defining Routes & Nested Routes
- Dynamic Routing & URL Parameters
- URL Parameters and Query Strings
- `useNavigate` Hook — Programmatic navigation
- Layout Components — Shared header/sidebar architecture
- Passing Data while Navigating
- Handling 404 Pages — fallback route for unmatched paths
- Folder Structure for Scalable Projects — `components/`, `hooks/`, `pages/`, `services/`, `utils/`

### 55. Server State & API Integration
- Fetch API Integration in React
- Handling Loading & Error States Gracefully
- Separation of Server State vs Client State
- Introduction to TanStack Query — Smart caching & refetching
- `useQuery` Basics — Data fetching pattern
- Mutations — Updating server data properly
- Sending form data to a backend using `fetch` or `axios`

### 56. Global State Management
- Context API — Managing app-wide state
- Context Providers & Consumers — Sharing state cleanly across deep component trees
- Zustand — Lightweight alternative to heavy Redux
- When to Use Global State vs Local State
- Avoiding Overengineering State Logic

### 57. State Management Using Redux
- Introduction to Redux — What is Redux?, When and Why use Redux?
- Understand Principles of Redux and Redux Flow
- Understanding State Management in React using Redux
- Why Use State Management Libraries?
- Why Redux needs reducers to be pure functions
- Redux Basics: Actions, Reducers, Store, Currying, Middleware, Async Actions: Thunk
- Connecting Redux to React Components with `react-redux`
- Introduction to Redux Toolkit
- Alternatives: Recoil, Zustand, or MobX

### 58. Advanced Forms & Validation
- Introduction to Forms in React
- Building Basic Forms — `input`, `textarea`, `select`, etc.
- Two-way binding with React
- Handling Form Events — `onChange`, `onSubmit`, `event.preventDefault()`
- Controlled vs Uncontrolled Forms
- React Hook Form — Efficient form handling
- Zod Schema Validation — Type-safe validation strategy
- Error Display Patterns
- Validation in React Forms — client-side form validation
- Integrating Forms with APIs
- Handling loading states and success/error feedback

### 59. Performance Optimization in React
- `React.memo` — Preventing unnecessary re-renders
- `useMemo` — Memoizing expensive calculations
- `useCallback` — Stable function references
- Code Splitting with `React.lazy` & `Suspense`
- Lighthouse Performance Testing
- Debugging Re-renders via DevTools
- Performance Profiling Tools — Chrome DevTools, Web Vitals, LCP, FID
- Avoiding Re-Renders using `useState`
- Optimizing Component Structure

### 60. TypeScript with React
- Understanding how TypeScript works with React
- Difference between `.ts` and `.tsx` files
- JSX typing fundamentals
- Typing functional components
- Understanding React typings ecosystem
- Props Typing — understanding props contracts, required/optional props, read-only props, children prop, reusable prop types, complex prop structures
- State Management Typing — typing component state, primitive vs object-based, nullable state, derived state, immutability
- Event Handling & Forms Typing — typing React events, mouse/keyboard events, form events, input and controlled form typing, validation/error state typing
- Context API with TypeScript — typing context values, provider/consumer, handling default values, scalable context architecture
- Redux with TypeScript — typing Redux store, reducers, actions, typed dispatch/selectors, Redux Toolkit with TypeScript
- API Integration & Data Typing — defining API data contracts, typing API responses, loading/success/error states, pagination/metadata typing, frontend-backend consistency
- Project Structure & Architecture — organizing React + TypeScript projects, feature-based folder structure, managing shared types, separation of concerns, scalable architecture patterns
- Common TypeScript Errors & Debugging

### 61. Deploying React Projects
- Preparing a React App for Production
- Building React Applications
- Environment Variables in React
- Deployment Platforms: Netlify, Vercel, GitHub Pages

### 62. Animations
- Animation and Transitions using libraries like `framer-motion` or `gsap` for advanced animations

### 63. Basic SEO Principles
- On-Page Optimization in SEO
- Guide to SEO Meta Tags
- Image SEO Best Practices
- Internal Link Building SEO
- Create An SEO Sitemap For a Website

### 64. Three.js and React Three-Fiber
- Understanding what is Scene
- Using 3D models for animation
- Controlling view with Orbit controls
- Applying Lights inside the scene
- Understanding different types of Cameras
- Animating the mesh with GSAP or Framer motion
- Different types of Geometries
- Using different Materials for animation

---

## Phase 7 — Next.js

### 65. Getting Started with Next.js
- Why Next.js is widely used for building modern web applications
- Next.js vs React — understanding the difference between a framework and a UI library
- What is Next.js and why it exists — problems Next.js solves in React applications
- Understanding client-side vs server-side rendering
- Setting up a new Next.js project using `create-next-app`
- Understanding File-Based Routing
- Understanding Next.js project structure
- Working with Layouts in Next.js
- Overview of Pages Router vs App Router

### 66. Routing in Next.js
- File-based routing system in Next.js
- Static routes
- Dynamic routes — `[id]`
- Nested routing structure
- Route grouping concepts
- Navigation using `next/link`
- Programmatic routing
- Handling 404 and error routes

### 67. Rendering Strategies in Next.js
- Server-Side Rendering (SSR) — generating pages on the server
- Static Site Generation (SSG) — pre-building pages for performance
- Incremental Static Regeneration (ISR) — updating static pages without rebuilding
- Client-Side Rendering (CSR)
- When to use which rendering method
- Data fetching strategies — `getStaticProps`, `getServerSideProps`, `getStaticPaths`
- Data fetching lifecycle in Next.js

### 68. Building APIs with Next.js
- Introduction to API routes in Next.js
- Using Next.js as a full stack framework
- Writing backend logic inside Next.js
- Implementing HTTP methods — GET, POST, PUT, PATCH, DELETE
- Connecting APIs with databases (MongoDB)
- Structuring responses and handling errors
- Creating authentication APIs
- Structuring API routes for scalability

### 69. Working with Server Actions
- Understanding Server Actions and how they differ from API routes
- Using the `use server` directive
- Implementing Server Actions for handling server-side logic

### 70. Styling & Assets in Next.js
- Global CSS handling
- Component-level styling with CSS Modules
- Integrating Tailwind CSS with Next.js
- Asset management in Next.js
- Image optimization using `next/image`
- Font optimization and font loading
- Metadata handling
- SEO optimization in Next.js applications

### 71. Next.js with TypeScript
- Using TypeScript with Next.js
- Typed pages and components
- Typed layouts
- Typing props and params
- Typed API routes
- Type safety in full stack Next.js apps

### 72. Middleware & Authentication in Next.js
- Introduction to middleware in Next.js
- Request and response interception
- Protecting routes using middleware
- Authentication flow in Next.js
- Auth using cookies
- JWT-based authentication
- Role-based access control

### 73. Deployment & Production (Next.js)
- Deploying Next.js applications
- Deployment using Vercel
- Environment variables management
- Production build optimization
- Performance optimization techniques
- Monitoring and debugging production issues

---

## Phase 8 — Node.js, Express & Backend Architecture

### 74. Starting with Node.js
- Introduction to Node.js and Getting Our Tools — Node.js LTS, Postman, Editor
- Setting up the Tools for our Environments
- Running script with Node.js — "Namaste Duniya"
- NPM Basics | Installing Packages
- Creating and Managing `package.json`

### 75. Creating Server — Writing Our First Server
- What is Server and how it works?
- Setting Up Our First Node.js Server using HTTP
- Serving A Response to the Browser and Understanding Responses
- Routing in HTTP Servers
- Understanding Status Codes — 1XX, 2XX, 3XX, 404, 200, 500, 422, 403, etc.
- Installing Nodemon for Automatic Server Restarts

### 76. Backend Architectures
- Different Architectures in backend — MVC and SOA
- Understanding MVC Architecture — Model, View, Controller
- MVC in the context of REST APIs

### 77. Web Framework — Express.js
- What is Express.js and why to use it
- Setting Up Express Server
- Returning Response from the server
- Using Query Parameters and URL Parameters
- HTTP Request — Different Types of Requests: GET, POST, PUT, PATCH, DELETE
- Serving Static Files with `express.static()`

### 78. Template Engine — EJS
- What is Template Engine and what is the use of Template Engine
- Template Engine Options — Handlebars, EJS, Pug, Jade
- Setting Up Template Engine — Installing EJS
- Rendering pages using EJS — `<%= %>`, `<% %>`, `<%- %>`
- Loop statement, Conditional statement and Locals in views
- Accessing Static Files Inside EJS file

### 79. Middleware in Express.js
- Understanding the middleware in Express
- Implementing middleware with Express
- Different types of middleware: built-in, third-party, custom
- Different levels of middleware: Application-Level, Router-Level
- Handling Errors and Security with middleware: Error-Handling, Helmet, CORS

### 80. Handling Files with Express
- Understand Multer and its use case
- Uploading file with Multer
- Understanding Memory and Disk Storage
- Accessing uploaded file `req.file`
- Working with `express.static`
- Using Cloudinary or ImageKit for Real-time media processing APIs and Digital Asset Management

### 81. Database Basics — MongoDB
- Relational and non-relational Databases: MongoDB & MySQL
- What is MongoDB? Why Use It?
- Installing Compass and accessing DB using terminal
- Setting Up MongoDB Locally and in the Cloud
- Understanding Datatypes, Collections and Documents
- Connecting MongoDB to Node.js with Mongoose
- Database Relations — One to One, One to Many, Many to Many, Polymorphic
- Handling Relationships with Mongoose (`populate`)

### 82. API Development (REST)
- What is a REST API?
- Versioning in RESTful APIs — `/v1/`
- Using Postman for API Testing and developing — Send Requests, Save Collections, Write Tests
- Understanding and Working With Status Codes — 2xx, 4xx, 5xx
- Validating API Inputs Using `express-validator` or Zod or Sanitization
- Proper error response format
- Security Handling — Rate Limiting with `express-rate-limit`, XSS Attack, CSRF Attack, DOS Attack

### 83. Input Validation
- Why validation matters
- `express-validator` OR Zod
- Sanitization
- Proper error response format

### 84. Database Optimization for Fast Response
- Indexing for Performance with MongoDB — Single-Field, Compound, Text, Wildcard Indexes
- Best practice with Indexing `explain()`
- Learning MongoDB Aggregation
- Comparison Operators — `$eq`, `$ne`, `$lt`, `$gt`, `$lte`, `$gte`, `$in`, `$nin`
- Logical Operators — `$not`, `$and`, `$or`, `$nor`
- Array Operators — `$pop`, `$pull`, `$push`, `$addToSet`
- Stages in Aggregation pipeline — `$match`, `$group`, `$project`, `$sort`, `$lookup`
- Creating Database on Local and Atlas
- Creating parallel pipeline with `$facet`
- Understanding Different types of Operators — Comparison, Regex, Update, Aggregation

### 85. Logging & Monitoring
- Why is Logging Important?
- Setting Up Logging with Libraries — Winston, Pino, Morgan
- Different modes of Morgan — `dev`, `short`, `tiny`
- Error Handling and Logging

### 86. Production Project Structure and Configuration
- Understanding the Basic Structure of application
- Learning File Naming Conventions, Git Configuration
- Understanding Important Folders — `src/`, `config/`, `routes/`, `utils/`
- Role of `package.json`, ENV and `.gitignore`
- Production Environment — PM2, Error & Response Handling Configuration, CORS Configuration, `async-handler.js`
- Using and Configuring ESLint and Prettier for code formatting
- Testing APIs using Postman

### 87. Authentication and Authorization
- Difference Between Authentication & Authorization
- Working with Passwords and Authentication — Cookie Authentication, OAuth Authentication
- Understanding Session and Token Authentication
- Implementing JWT Authentication — `jsonwebtoken`, `JWT_SECRET`
- Securing user password with `bcrypt` hashing salt
- Role-Based Access Control (RBAC)
- Authenticating user with Express middleware
- Understanding Passport.js and its use case
- Setting up Passport.js — `passport-local`, `local-strategy`, `google-OAuth`
- `express-sessions` and using passport for authentication

### 88. Real-time Communication — WebSockets and Socket.io
- Understanding WebSockets protocol for real-time applications
- Learning handshake, Persistent connection, Bidirectional communication, HTTP polling
- Understanding difference between WebSocket vs Socket.io
- Working with Socket.io for real-time applications
- Understanding usage of Rooms in Socket.io
- Understanding Middleware in Socket.io

### 89. Working with Caching — Local and Redis
- What is Caching and How to cache data locally?
- What is Redis?
- Why Use Redis for Caching?
- Implementing Redis Caching in Node.js
- Advanced Redis Features — TTL, Complex Data Structures, Pub/Sub

### 90. Error Handling in Express
- Basic Error Handling in Express `next()`
- Catching Specific Errors `try` & `catch`
- Creating Util Class for Error Handling

### 91. Testing Tools
- Understanding Unit-Testing With Jest
- Cross Browser Testing and Why Is It Performed?
- What Is Web Testing? and How to Test a Website

---

## Phase 9 — Generative AI Engineering

### 92. How LLMs Actually Work
- What is Generative AI and how it works (ML, DL, and LLM concepts)
- Core models behind Generative AI — Transformers, Diffusion Models, GANs
- What are Tokens and why everything becomes tokens
- What is Context Window and why prompts get cut
- Sampling Basics — temperature and randomness control
- Why Hallucination happens (it predicts, it doesn't "know")
- Difference between Deterministic vs Probabilistic outputs
- Understanding use-cases and limitations (bias, hallucination, accuracy)

### 93. Calling LLM APIs Properly
- Message roles — `system`, `user`, `assistant`
- Token budgeting — prompt size, response size, and overflow planning
- Cost awareness — pricing per token and why bad prompts waste money
- Rate limits — handling `429`, backoff and retries

### 94. Prompt Engineering Fundamentals
- Write clear instructions (don't be vague)
- Few-shot examples to force pattern learning
- Chain-of-thought: high-level awareness
- Output formatting instructions (make the response predictable)
- Prompt Optimization using tools

### 95. Structured Output in AI Systems
- Why unstructured AI responses are difficult to use in real systems
- How structured responses make AI outputs predictable and programmable
- Common applications — resume parsing, product metadata generation, moderation systems, compatibility scoring engines

### 96. Generating JSON Responses from LLMs
- Using model-supported JSON mode for structured outputs
- Guiding models with schema-based prompting
- Basics of tool/function calling
- Validating the returned structure before using it
- Building examples where AI returns structured data

### 97. Schema Validation with Zod
- Defining a validation schema using Zod
- Verifying AI responses against a schema
- Handling invalid or mismatched responses
- Implementing retry strategies for broken outputs
- Principle: never trust AI output without validation

### 98. Function Calling / Tool Calling
- What is tool calling and why it matters
- When to use it (deterministic actions)
- Deterministic tool invocation
- Hybrid logic (AI + code)
- Making AI decide which function to call

### 99. Streaming Responses
- Streaming tokens from the model instead of waiting for full output
- Progressive rendering in user interfaces
- Improving UX in AI-driven applications
- Combining Streaming with Structured Data
- Streaming explanation or conversational text
- Returning structured JSON data once generation finishes
- Separating UI responses from system-readable outputs

### 100. Error Handling in AI Applications
- Handling invalid or malformed JSON responses
- Managing partial responses and timeouts
- Implementing retry mechanisms
- Logging AI requests and responses for debugging

### 101. Understanding Embeddings & Vector Databases
- What embeddings represent in vector space
- How similarity search works conceptually
- Document chunking strategies for better retrieval
- Storing embeddings for search and retrieval
- Querying similar vectors efficiently
- Using metadata filters during search

### 102. Building a RAG Pipeline
- Basic RAG workflow: User query → Retrieve relevant chunks → Inject into prompt → Structured answer
- Build: Document QA system returning structured JSON

### 103. Evaluating AI Systems
- Detecting hallucinations
- Assigning confidence scores
- Evaluating retrieval quality
- Observability and monitoring basics

### 104. Understanding AI Agents
- Agent vs single LLM call
- Agent = reasoning + tool usage
- When to use multi-agent systems
- When NOT to use them
- Multi-agent systems increase complexity

### 105. Agent Design Patterns
- Planner → Executor workflow
- Researcher → Writer pattern
- Critic → Refiner loop
- Router agents that decide which tool to call

### 106. LangChain (Practical)
- Introduction to LangChain and its features
- Building chains and prompt templates
- Using tools and memory modules
- Working with agents
- Overview of LCEL concepts
- Working with LLM Chains, Memory, and Tools

### 107. Building Multi-Agent Workflows
- Multi-agent examples (Profile Analyzer, Bio Improver, Conversation Starter Generator, Image Metadata Extractor, SEO Optimizer, Tag Categorizer)
- Pipeline: Input → Analyze → Improve → Generate → Structured JSON output
- All outputs validated with schema

### 108. Multi-Agent Architecture Concerns
- Increased latency
- Higher operational cost
- Debugging difficulty across agents
- Managing shared state between services
- Importance of logging each step in the pipeline
- Understanding that multi-agent systems are not always the best solution

### 109. Building Real-World AI Applications
- Building an Authentication System with Generative AI
- Creating Social Media Automation Tools (AI post generator, auto-scheduler)
- Developing Content Generation Projects (blog writer, idea generator)
- AI-powered Resume Reviewer (using ChatGPT or Gemini API)
- Virtual Interview Assistant using LLM APIs + Voice/Prompt Engineering
- Exploring Agentic-AI Applications (multi-step reasoning systems)
- Overview of MCP Server (Model Context Protocol) and its role in LLM interoperability

### 110. AI Extras (Lovable AI Project)
- Try to use Free Models of Ollama, HuggingFace and get the Deployment Idea about these models
- Filter the unusual prompts given to model by User — learn approaches about it

---

## Phase 10 — Progressive Web Apps (PWA)

### 111. Understanding PWAs
- What are Progressive Web Apps and why they matter
- Benefits: Offline access, app-like experience, installability
- Real-world examples: Twitter Lite, Starbucks PWA

### 112. Core Components of a PWA
- Service Workers: Role, lifecycle, and registration
- Lifecycle stages: Install, Activate, Fetch
- Handling caching and background sync
- Manifest File: Purpose and structure — `name`, `short_name`, `icons`, `start_url`, `theme_color`, `background_color`
- DevTools for Debugging: Application tab, cache inspection, and audit tools

### 113. PWA Performance Optimization
- Implementing Lazy Loading and Code Splitting
- Testing PWA with Lighthouse
- Advanced caching strategies (Cache First, Network First, Stale-While-Revalidate)
- Techniques for faster load time and smoother offline experiences

---

## Phase 11 — DevOps, Infrastructure & Deployment

### 114. DevOps Foundations
- What is DevOps and why it's essential
- Understanding the difference between development and operations
- Stages: Plan → Build → Test → Release → Deploy → Monitor → Feedback
- Basics of CI and CD for automated builds and deployments
- Introduction to Infrastructure as Code (IaC)
- Why applications behave differently in Production vs Localhost
- Understanding Development, Staging, and Production environments
- Basic Linux usage and connecting to servers using SSH
- Important Linux commands — `ls`, `cd`, `mkdir`, `nano`, `vim`, `ps`, `kill`, `top`
- Managing backend applications in production using PM2
- Running Node.js apps in background and monitoring logs

### 115. Docker & Containerization
- Introduction to Docker and container-based deployments
- Understanding Images vs Containers
- What are containers and how they differ from virtual machines
- Why containers improve consistency across environments
- Core Docker concepts: Image, Container, Volume, Network
- Writing a simple Dockerfile using `FROM`, `WORKDIR`, `COPY`, `RUN`, `EXPOSE`, `CMD`
- Containerizing a backend service
- Running multi-service apps using Docker Compose
- Connecting services like Backend, MongoDB, and Redis
- Optimizing builds using multi-stage Docker builds and `.dockerignore`

### 116. Cloud Deployments
- Basics of Cloud Computing
- Overview of major cloud providers — AWS, GCP, Heroku, Azure, DigitalOcean
- Understanding scalability, high availability, and fault tolerance
- Managing infrastructure cost and performance

### 117. AWS EC2
- Introduction to AWS cloud platform
- Understanding regions and availability zones
- What EC2 instances are and how they work
- Launching and configuring an EC2 instance
- Connecting to EC2 using SSH
- Installing Node.js and Docker on the server
- Deploying a backend service manually
- Cloning the repository and running the production build
- Configuring NGINX as a reverse proxy
- Masking the Domain Name to the server IP (DNS configuration)

### 118. Security Groups
- What Security Groups are and why they matter
- Managing inbound and outbound rules
- Restricting server access for security
- Security best practices

### 119. Load Balancers
- What a Load Balancer does
- Why load balancing improves reliability
- Using AWS Elastic Load Balancer
- Configuring Application Load Balancer (ALB)
- Health checks for monitoring services

### 120. AWS CloudFront
- Introduction to CloudFront
- Using CDN for faster content delivery
- Caching and edge locations
- Serving static assets efficiently

### 121. CI/CD Automation
- Understanding Continuous Integration
- Creating workflows with GitHub Actions (and Jenkins)
- Running tests and build pipelines
- Automating deployments
- Triggering deployments on `git push`
- Deploying to servers via SSH
- Rebuilding Docker containers automatically

### 122. Kubernetes — Orchestration
- What is Kubernetes (K8s) and why it's used for scaling microservices
- Core components: Pod, Deployment, ReplicaSet, Service, Ingress
- Managing workloads and ensuring high availability
- Setting up Minikube or Docker Desktop Kubernetes locally
- Deploying a microservice on Kubernetes
- Load balancing and auto-scaling with Kubernetes
- Deploying microservices using Kubernetes clusters on AWS EKS
- Managing secrets and environment variables with Kubernetes Secrets & ConfigMaps

### 123. Terraform — Infrastructure as Code (IaC)
- What is Terraform and how it automates cloud infrastructure
- Understanding Providers, Resources, and State Management
- Writing basic `.tf` files to provision AWS EC2 instances
- Using Terraform with Docker and Kubernetes deployments
- Real-world scenario: Automate deployment of a Node.js + MongoDB app to AWS using Terraform

### 124. Scalability & Reliability
- Vertical vs Horizontal scaling
- Load balancing strategies
- Using Redis for caching
- Importance of stateless backend design
- Understanding sticky sessions and when to avoid them
- Monitoring, logging, and observability basics

### 125. Caching in Production
- Using Redis for application caching
- Understanding the cache invalidation challenge
- Applying TTL strategies to manage cache lifetime
- Preventing stale or outdated cached data

### 126. Logging & Observability
- Using Structured Logging for backend systems
- Monitoring application logs and system metrics
- Understanding basic observability principles
- Introduction to alerting systems
- Logging important events — API errors, authentication failures, AI usage

### 127. Production Hardening
- Strengthening backend security for production environments
- Implementing rate limiting for APIs
- Proper CORS configuration
- Understanding DDoS protection concepts
- Using secure HTTP headers

### 128. Final Production Deployment
- Deploying a complete system using Docker
- Running services on EC2
- Connecting a domain with SSL
- Automating deployments using CI/CD pipelines
- Using DigitalOcean App Platform (auto-scaling, containers, built-in load balancer)
- CI/CD pipeline integration: Deploy code → Build Docker image → Push to registry → Deploy via Terraform → Orchestrate with Kubernetes

---

## Phase 12 — Microservices & Scaling

### 129. Microservice Foundations
- Understanding Monolithic vs Microservices architecture
- When microservices make sense and when they add unnecessary complexity
- Identifying proper service boundaries using domain-based thinking
- The Database-per-Service principle in distributed systems
- Communication approaches — synchronous (REST) and asynchronous (Events)
- Key benefits: Scalability, modularity, independent deployment
- Common challenges (data sharing, inter-service communication, debugging)

### 130. Building & Orchestrating Microservices
- Creating independent services with separate codebases and configurations
- Running multiple backend services as separate Node.js applications
- Structuring microservices with individual `package.json`
- Designing microservice architecture for a sample app (e.g., eCommerce system)
- Understanding the API Gateway pattern for centralized routing and authentication
- Forwarding requests from client → gateway → internal services
- Handling internal service communication using REST calls
- Retry strategies, timeouts, and circuit breaker concepts
- Introduction to event-driven architecture
- Using RabbitMQ/Redis Pub/Sub for event communication
- Designing event payloads and ensuring idempotency
- Understanding eventual consistency in distributed systems
- Proxying requests, rate limiting and authentication at gateway level
- Dockerizing and deploying microservices
- Overview of Kubernetes orchestration for microservice clusters

### 131. AWS Cloud-Native Deployment
- Using Amazon ECR to store and manage container images
- Building Docker images locally and pushing them to ECR
- Understanding ECS clusters and task definitions
- Overview of Fargate vs EC2 container execution
- Routing traffic using Application Load Balancer (ALB)
- Configuring target groups and service health checks
- Understanding VPC, Subnets, and network security groups
- Basic introduction to IAM roles and permissions

### 132. Distributed Observability & Scaling
- Scaling backend services horizontally using ECS tasks
- Understanding stateless service architecture
- Using health checks to manage service availability
- Monitoring services with CloudWatch
- Observing system resilience by simulating service failures
- Tracking AI usage and system events through service logs

---

## Phase 13 — Web3 Basics (Introductory)

### 133. Web3 Fundamentals
- Understanding the concept and potential of Web3
- Fundamentals of Blockchain technology and how it powers Web3
- Exploring Decentralized Applications (DApps) and their use cases
- Introduction to Smart Contracts: How they work and their applications
- Overview of Cryptocurrencies and their role in the Web3 ecosystem

---

## Phase 14 — System Design

### Low Level Design (LLD)

### 134. LLD Foundations
- What is Low Level Design (code-level system breakdown)
- Understanding OOP (classes, objects, inheritance, polymorphism)
- How to think in class relationships and object interactions
- Basics of UML Diagrams (class diagrams, sequence diagrams)
- How to approach LLD interviews step-by-step

### 135. Design Principles
- SOLID Principles (core of maintainable code)
- DRY — avoid duplication
- Introduction to Design Patterns
- Writing extensible and scalable code

### 136. Creational Design Patterns
- Singleton — one instance control
- Factory Method — object creation abstraction
- Abstract Factory — families of related objects
- Builder — step-by-step object creation
- Prototype — cloning objects efficiently

### 137. Structural Design Patterns
- Adapter — compatibility between interfaces
- Facade — simplified interface over complex system
- Proxy — controlled access
- Decorator — dynamic behavior extension
- Composite — tree-like object structures

### 138. Behavioral Design Patterns
- Observer — event-based updates
- Strategy — interchangeable logic
- Command — encapsulate actions
- Iterator — sequential access
- State — behavior changes with state
- Template Method — define skeleton logic
- Chain of Responsibility — request flow handling
- Mediator — centralized communication

### 139. LLD Problem Solving (Machine Coding)
- Designing Parking Lot System
- Designing Vending Machine
- Designing BookMyShow
- Designing Splitwise
- Designing Uber / Ola
- Designing Elevator System

### High Level Design (HLD)

### 140. System Design Foundations
- What is High Level Design (system architecture overview)
- Understanding functional vs non-functional requirements
- How to break systems into components & services
- Capacity estimation basics (users, traffic, storage)
- Step-by-step system design interview approach
- Core Performance Concepts — latency, throughput
- Understanding scalability, performance, reliability, availability, fault tolerance

### 141. Communication & Data Layer
- Basics of Networking (HTTP, TCP, latency)
- Designing clean APIs (REST principles)
- SQL vs NoSQL — when to use what
- Database scaling (replication, sharding basics)
- Managing data consistency vs performance
- Data Replication — leader-follower, multi-leader, read replicas
- Data Sharding — shard keys, range-based, hash-based

### 142. Core Infrastructure
- Caching strategies (Redis, in-memory, client-side, server-side, database cache, CDN cache)
- CDN and content delivery optimization (edge caching, static assets)
- Load Balancing (horizontal scaling, health checks, layer 4 vs layer 7 routing)
- API Gateway role in distributed systems
- Message Queues (async communication, event-driven, producers, consumers, Kafka)
- Microservices Architecture fundamentals
- Stateless vs Stateful Systems — session handling, server independence

### 143. Advanced Distributed Systems
- Reliability and system availability
- Fault Tolerance and failure handling
- High Availability Concepts — redundancy, failover, auto-scaling
- Observability (logs, metrics, tracing)
- Rate Limiting and traffic control
- Authentication & Authorization
- Designing Search Systems
- Data Migration — schema changes, versioning, online migration, zero-downtime migration
- Monitoring & Observability — logging, metrics, tracing

### 144. Real-World System Design Problems
- 12 real-world system design problems

---

## Phase 15 — Capstone Projects

### Project 1: Lovable AI — AI-Assisted Product Builder

**1. Account & Setup**
- Sign up, Log in, Log out, Reset password, Basic profile details

**2. Project Workspace**
- Create new project, Project dashboard, Project description
- Edit project details, Delete project, Recent projects list

**3. Prompt Input**
- Enter project prompt, Prompt history, Edit prompt
- Regenerate response, Save prompt versions

**4. AI Agent Collaboration**
- Multiple agents responding to one prompt
- Agents with different roles
- View agent responses separately
- Combined solution view
- Regenerate individual agent response

**5. Generated Output**
- View generated code or content
- Structured output view
- Copy generated output, Download generated files
- Regenerate output

**6. Iteration & Refinement**
- Follow-up prompt, Improve existing output
- Update generated result
- Prompt version history, Compare previous outputs

**7. File & Project Structure**
- Generated file list, Open file preview
- Edit generated content, Save file changes
- Download project files

**8. Collaboration & Organization**
- Project activity history, Prompt interaction timeline
- Organize projects, Search projects

**9. User Experience**
- Loading indicators during generation
- Streaming responses, Clean workspace layout
- Dark mode, Notifications for generation completion

**10. Basic AI Controls**
- Select number of agents, Choose agent roles
- Regenerate individual agent, Stop generation

**11. Extras**
- Prompt Optimization using tools
- Use Free Models of Ollama, HuggingFace — deployment ideas
- Filter unusual/harmful prompts — learn moderation approaches

---

### Project 2: ImageKit — Media Processing & Delivery Platform

**1. Account & Setup**
- Sign up, Log in, Log out, Reset password, Basic profile details

**2. Media Upload**
- Upload images, Upload videos
- Drag & drop upload, Multiple file upload
- Upload progress indicator, File size limit warning

**3. Media Library**
- Grid view, List view
- Folder creation, Move files between folders
- Rename files, Delete files
- Sort by date, Sort by size
- Search files by name

**4. Media Preview**
- Full image preview, Video preview
- Zoom in/out, File details panel
- Download file, Copy file link

**5. Image Editing (Basic)**
- Resize image, Crop image, Rotate image
- Change quality
- Convert format (JPG / PNG / WEBP)

**6. Organization & Management**
- Favorite files, Recently uploaded section
- Trash folder, Restore deleted files, Permanent delete
- Tag files, Filter by file type

**7. Sharing & Access**
- Share via link
- Public / private file setting
- Link expiry option
- View-only access, Download permission control
- Signed URL for accessing

**8. Storage Insights**
- Total storage used, File size breakdown
- Number of uploads, Storage limit warning

**9. User Experience Enhancements**
- Loading placeholders, Smooth animations
- Infinite scroll, Dark mode
- File upload notifications, Clean dashboard layout

**10. Medium-Level Advanced Features**
- Bulk file actions, Duplicate file detection
- Image compression before upload
- Folder color labels, Smart search filters
- Recent activity log

**11. Extras**
- Network Optimization
- Advanced file transformation
- Migration from ImageKit, Cloudinary, AWS
- Bucket integration (S3)
- Amazon CloudFront CDN integration — sub-500ms latency target
- Caching strategies for media delivery
- URL-based transformation parameters
