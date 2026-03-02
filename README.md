# Full Stack Web Development: 26-Week Project-Based Learning Plan

## 📋 Overview & Philosophy

This plan follows **just-in-time learning**: you learn a concept only when you need it to build something. Each week introduces new skills through a project that builds on everything before it. You'll go from zero to deploying a production-grade full-stack application.

**Tech Stack Choice:** HTML → CSS → JavaScript → React → Tailwind CSS → Node.js/Express → PostgreSQL → Redis → Docker → AWS

**Weekly Time Commitment:** 15–25 hours/week

**How to Use This Plan:**
1. Read the week's overview and project description
2. Research the listed concepts *just enough* to start building
3. Build the project — get stuck, search, debug, repeat
4. Complete the stretch challenges before moving on
5. Commit everything to GitHub

---

## 🟢 PHASE 1: FOUNDATIONS (Weeks 1–6)

---

### **WEEK 1: The Internet & Your First Webpage**
**🎯 Project: Personal "About Me" Webpage**

**Concepts to Learn (Just-in-Time):**
- How does the internet work? (Client-server model, HTTP requests)
- What is a domain name, DNS, and hosting?
- How do browsers render pages?
- HTML basics: elements, tags, attributes, document structure
- Setting up VS Code (or any code editor)

**Project Details:**
Build a single-page "About Me" website using only HTML. No CSS, no JavaScript — pure HTML.

**Requirements:**
- Proper `<!DOCTYPE html>` declaration and document structure (`<html>`, `<head>`, `<body>`)
- A heading with your name
- A paragraph about yourself
- An image (of anything — yourself, a pet, a landscape)
- A list of 5 hobbies (unordered list)
- A list of your education or work experience (ordered list)
- A table showing your weekly schedule
- A navigation section with links to different parts of the page (use anchor `#id` links)
- A contact section with a basic form (name, email, message fields) — it won't submit anywhere yet
- Use semantic HTML tags: `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>`

**Step-by-Step Guidance:**
1. Create a folder called `about-me` on your computer
2. Inside it, create a file called `index.html`
3. Open it in VS Code. Type `!` and press Tab — VS Code will generate a basic HTML template
4. Open the file in your browser (just double-click it, or right-click → "Open with" → Chrome)
5. Start adding elements one by one. After each addition, refresh your browser to see changes
6. When you get stuck on a tag, search "MDN [tag name]" — MDN Web Docs is your best friend

**🤔 Think About:**
- What's the difference between `<div>` and `<section>`? When would you use each?
- Why does semantic HTML matter? (Hint: think about screen readers and SEO)
- What happens when you open your HTML file — is a server involved?

**Stretch Challenges:**
- Add a `<details>` and `<summary>` element for a FAQ section
- Add `<meta>` tags for description and viewport
- Validate your HTML at [validator.w3.org](https://validator.w3.org/)

**📚 Resources to Search For:**
- "MDN HTML basics tutorial"
- "How the internet works in 5 minutes" (YouTube)
- "What is HTTP" (freeCodeCamp)

---

### **WEEK 2: Styling with CSS**
**🎯 Project: Styled Personal Portfolio Page**

**Concepts to Learn (Just-in-Time):**
- CSS syntax: selectors, properties, values
- The box model (margin, border, padding, content)
- CSS layouts: Flexbox and CSS Grid
- Responsive design with media queries
- CSS units: px, em, rem, %, vh, vw
- Colors, fonts, and typography
- The cascade, specificity, and inheritance

**Project Details:**
Take your Week 1 HTML page and transform it into a beautiful, responsive portfolio page using CSS.

**Requirements:**
- Create an external stylesheet (`styles.css`) linked to your HTML
- A fixed or sticky navigation bar at the top
- A hero section with a large heading, subtitle, and a background color or gradient
- A two-column layout for an "About + Photo" section (stacks vertically on mobile)
- Style the hobbies list as a grid of cards with hover effects
- Style the table with alternating row colors
- Style the form with proper spacing, borders, and a styled submit button
- The page must look good on mobile (≤ 480px), tablet (≤ 768px), and desktop (≥ 1024px)
- Smooth scroll behavior for navigation links
- At least one CSS transition (e.g., button hover, card hover)
- Use a Google Font

**Step-by-Step Guidance:**
1. Create `styles.css` in your project folder
2. Link it in your HTML `<head>`: `<link rel="stylesheet" href="styles.css">`
3. Start with a CSS reset or normalize (search "CSS reset 2024")
4. Style the page top-to-bottom: navigation first, then hero, then each section
5. Build the layout with Flexbox first — try Grid for the hobbies cards section
6. Add media queries last, after the desktop version looks good
7. Use Chrome DevTools (F12) → toggle device toolbar to test responsive design

**🤔 Think About:**
- When should you use Flexbox vs. Grid? Can you articulate the difference?
- What does `box-sizing: border-box` do and why does almost everyone use it?
- If two CSS rules conflict, how does the browser decide which to apply?

**Stretch Challenges:**
- Add a dark mode toggle using a CSS class (you'll manually toggle it in DevTools for now)
- Add CSS animations (keyframes) to animate elements when the page loads
- Try recreating a design from [dribbble.com](https://dribbble.com) for your portfolio layout
- Learn about BEM naming convention and refactor your class names

**📚 Resources to Search For:**
- "CSS Flexbox guide" (css-tricks.com — A Complete Guide to Flexbox)
- "CSS Grid guide" (css-tricks.com — A Complete Guide to Grid)
- "CSS media queries tutorial"
- "Chrome DevTools for beginners"

---

### **WEEK 3: JavaScript Fundamentals**
**🎯 Project: Interactive Quiz Application**

**Concepts to Learn (Just-in-Time):**
- JavaScript data types, variables (`let`, `const`), operators
- Functions (declarations, expressions, arrow functions)
- Control flow: if/else, switch, ternary operator
- Loops: for, while, forEach, map, filter
- Arrays and Objects
- DOM manipulation: `querySelector`, `getElementById`, `addEventListener`
- Events: click, submit, input, keydown
- Template literals
- Basic debugging with `console.log` and browser DevTools

**Project Details:**
Build an interactive quiz app that presents questions one at a time, tracks the score, and shows results at the end. All HTML/CSS/JS — no frameworks, no libraries.

**Requirements:**
- At least 10 questions stored in a JavaScript array of objects
- Each question object should have: question text, array of answer options, correct answer index
- Display one question at a time with multiple-choice answers as clickable buttons
- Highlight the selected answer (green for correct, red for incorrect)
- Show a "Next" button after answering
- Display a progress bar or question counter (e.g., "Question 3 of 10")
- Track and display the score
- Show a results screen at the end with score, percentage, and a "Restart" button
- The quiz data should be separate from the display logic (separation of concerns)

**Step-by-Step Guidance:**
1. Create a new project folder: `quiz-app/` with `index.html`, `styles.css`, `script.js`
2. First, design the HTML structure: a container for the quiz, question area, answer buttons, navigation
3. Style it to look clean and centered on the page
4. In `script.js`, start by creating your quiz data:
```javascript
const quizData = [
  {
    question: "What does HTML stand for?",
    options: ["Hyper Text Markup Language", "High Tech ML", "Hyper Transfer ML", "None"],
    correct: 0
  },
  // ... more questions
];
```
5. Write a function `loadQuestion(index)` that updates the DOM with the current question
6. Add event listeners to answer buttons
7. Write functions for checking answers, updating score, moving to next question
8. Write a function to show final results

**🤔 Think About:**
- What is the DOM and how does JavaScript interact with it?
- What's the difference between `let`, `const`, and `var`? When should you use each?
- Why is it a bad idea to put quiz answers directly in the HTML? (Hint: view source)
- What would happen if you needed 1000 questions? How would your data structure need to change?

**Stretch Challenges:**
- Add a timer for each question (15 seconds to answer)
- Add different difficulty levels
- Randomize question order each time the quiz starts
- Store the high score in `localStorage` so it persists across browser sessions
- Add keyboard navigation (press 1, 2, 3, 4 to select answers)

**📚 Resources to Search For:**
- "JavaScript.info" (comprehensive modern JS tutorial)
- "MDN JavaScript basics"
- "DOM manipulation JavaScript tutorial"
- "JavaScript array methods explained"

---

### **WEEK 4: Advanced JavaScript & Version Control**
**🎯 Project: Task Manager (To-Do App) with Local Storage + Git Setup**

**Concepts to Learn (Just-in-Time):**
- Git basics: init, add, commit, status, log, diff, .gitignore
- GitHub: creating repos, pushing code, README.md writing (Markdown)
- ES6+ features: destructuring, spread operator, rest parameters, optional chaining
- Higher-order functions: map, filter, reduce, sort
- Local Storage API
- JSON: parse and stringify
- Error handling: try/catch
- Closures and scope (basic understanding)
- Event delegation

**Project Details:**
Build a feature-rich task manager application. This is also the week you start using Git for everything.

**Git Setup (Do This First):**
1. Install Git on your computer
2. Configure your name and email: `git config --global user.name "Your Name"`
3. Create a GitHub account
4. Go back and create repos for your Week 1, 2, and 3 projects — push them all to GitHub
5. For this week's project, initialize Git from the start: `git init`
6. Make small, meaningful commits as you build each feature

**Project Requirements:**
- Add tasks with a title, description, priority (low/medium/high), and due date
- Display tasks in a list with visual indicators for priority (colors)
- Mark tasks as complete (strikethrough + move to "completed" section)
- Edit existing tasks (click to edit inline or in a modal)
- Delete tasks with a confirmation prompt
- Filter tasks: All, Active, Completed
- Sort tasks by: date added, due date, priority
- Search/filter tasks by keyword
- All data persists in localStorage — tasks survive page refresh
- Show task count ("3 active tasks, 2 completed")
- Use event delegation on the task list (don't add individual listeners to each task)

**Git Commit Strategy:**
Make commits at each meaningful milestone:
- "Initial project structure with HTML/CSS"
- "Add task creation functionality"
- "Implement localStorage persistence"
- "Add edit and delete features"
- "Add filtering and sorting"
- etc.

**🤔 Think About:**
- Why use event delegation instead of adding listeners to each task element?
- What happens if localStorage is full or disabled? How would you handle that?
- How would you structure your code if this app grew to have 50 features? (Think about modules)
- What makes a good Git commit message?

**Stretch Challenges:**
- Add drag-and-drop to reorder tasks
- Add categories/tags for tasks
- Add a "due today" and "overdue" section with visual warnings
- Export tasks as JSON file (download)
- Import tasks from a JSON file (file upload)
- Create a GitHub README with screenshots and description of your project

**📚 Resources to Search For:**
- "Git tutorial for beginners" (Atlassian or freeCodeCamp)
- "GitHub getting started guide"
- "localStorage JavaScript tutorial"
- "Event delegation JavaScript explained"
- "How to write a good README"

---

### **WEEK 5: CSS Frameworks & Package Managers**
**🎯 Project: Weather Dashboard with Tailwind CSS**

**Concepts to Learn (Just-in-Time):**
- npm: what it is, `package.json`, installing packages, `node_modules`, `.gitignore` for `node_modules`
- Tailwind CSS: utility-first approach, installation, configuration
- Fetching data from APIs: `fetch()`, Promises, `async/await`
- Working with JSON data from external APIs
- Error handling for network requests
- Environment variables (basic concept — don't commit API keys!)

**Project Details:**
Build a weather dashboard that fetches real weather data from a free API and displays it beautifully using Tailwind CSS.

**Setup Steps:**
1. Create new project folder
2. Run `npm init -y` to create `package.json`
3. Install Tailwind CSS following the official docs (use the CLI method)
4. Sign up for a free API key at [OpenWeatherMap](https://openweathermap.org/api) or [WeatherAPI](https://www.weatherapi.com/)
5. Initialize Git and create `.gitignore` (include `node_modules/` and any `.env` file)

**Requirements:**
- Search bar to look up weather by city name
- Display current weather: temperature, humidity, wind speed, condition (sunny/cloudy/etc.), weather icon
- Display a 5-day forecast with daily high/low temperatures
- Show "feels like" temperature, visibility, and pressure
- Dynamic background or theme that changes based on weather condition (sunny = warm colors, rainy = cool colors)
- Loading state while fetching data (spinner or skeleton)
- Error handling: show a user-friendly message if the city is not found or the API fails
- Display the last searched city on page load (use localStorage)
- Fully responsive: looks great on mobile and desktop
- Built entirely with Tailwind CSS utility classes — no custom CSS file (except Tailwind's base)

**🤔 Think About:**
- What is a Promise? How does `async/await` relate to Promises?
- What happens if the API is slow or down? How should your app handle that?
- Why shouldn't you commit API keys to GitHub? What could go wrong?
- What are the pros and cons of utility-first CSS (Tailwind) vs. traditional CSS?

**Stretch Challenges:**
- Add geolocation to detect the user's current location and show their weather automatically
- Add unit toggle (Celsius ↔ Fahrenheit)
- Show a map with the city location (use Leaflet.js or a simple embedded map)
- Add "favorite cities" that persist in localStorage
- Show hourly forecast for the current day
- Add weather alerts if available from the API

**📚 Resources to Search For:**
- "Tailwind CSS tutorial for beginners"
- "JavaScript fetch API tutorial"
- "async await JavaScript explained"
- "npm for beginners"
- "OpenWeatherMap API tutorial"

---

### **WEEK 6: Checkpoint & Consolidation Project**
**🎯 Project: Personal Portfolio Website (Production-Quality)**

**Concepts to Learn (Just-in-Time):**
- Responsive images and performance optimization
- CSS animations and micro-interactions
- Accessibility (a11y): ARIA labels, keyboard navigation, color contrast
- SEO basics: meta tags, Open Graph, semantic structure
- Deploying static sites: GitHub Pages, Netlify, or Vercel
- Custom domain setup (optional, but learn how it works)

**Project Details:**
Build a polished, portfolio website to showcase your first 5 projects. This is your first "production" deploy — it will be live on the internet.

**Requirements:**
- **Home/Hero:** Your name, title ("Aspiring Full Stack Developer"), a professional tagline, and a call-to-action button
- **About:** Short bio, your tech skills with visual indicators (skill bars or icons)
- **Projects Section:** Cards for each of your previous projects with:
  - Screenshot/thumbnail
  - Project name and description
  - Technologies used (as tags/badges)
  - Links to live demo and GitHub repo
- **Contact:** A working contact form (use [Formspree](https://formspree.io/) or [EmailJS](https://www.emailjs.com/) to make it actually send emails)
- **Navigation:** Smooth scrolling, mobile hamburger menu
- **Footer:** Social links (GitHub, LinkedIn, etc.)
- Accessible: passes basic accessibility checks
- SEO-optimized: proper meta tags, Open Graph tags for social sharing
- Performance: optimized images, minimal render-blocking resources
- **Deployed and live** on the internet with a shareable URL

**Deploy Steps:**
1. Push your code to GitHub
2. Option A: Use GitHub Pages (Settings → Pages → Deploy from branch)
3. Option B: Connect your repo to Netlify or Vercel for automatic deploys
4. Share the live URL!

**🤔 Think About:**
- If someone shares your portfolio link on Twitter/LinkedIn, what shows up? (Open Graph tags)
- Can a blind person navigate your site using a screen reader?
- How fast does your site load? Run Lighthouse in DevTools and try to score > 90 on all categories

**Stretch Challenges:**
- Add a blog section with markdown-like formatted posts
- Add dark/light theme toggle that remembers the user's preference
- Add page transition animations
- Score 90+ on all Lighthouse categories (Performance, Accessibility, Best Practices, SEO)
- Buy a custom domain and connect it

---

## 🟡 PHASE 2: FRONTEND FRAMEWORK (Weeks 7–12)

---

### **WEEK 7: React Fundamentals**
**🎯 Project: Movie Search App**

**Concepts to Learn (Just-in-Time):**
- What is React and why use it? (Component-based architecture, Virtual DOM)
- Create React App vs. Vite (use Vite — it's faster)
- JSX syntax
- Components: functional components
- Props: passing data down
- State: `useState` hook
- Rendering lists with `.map()` and the `key` prop
- Handling events in React
- Conditional rendering

**Project Setup:**
```bash
npm create vite@latest movie-search -- --template react
cd movie-search
npm install
npm run dev
```

**Project Details:**
Build a movie search application using the [OMDB API](http://www.omdbapi.com/) (free API key) or [TMDB API](https://www.themoviedb.org/documentation/api).

**Requirements:**
- A search bar component that takes user input
- Display search results as a grid of movie cards
- Each movie card shows: poster image, title, year, rating
- Click on a movie card to see detailed information (you can show it in a modal or a separate section of the page)
- Loading state while fetching
- Error/empty states ("No movies found", "Something went wrong")
- Debounce search input (bonus concept!) so you don't make an API call on every keystroke

**Component Structure (suggested):**
```
App
├── SearchBar
├── MovieGrid
│   └── MovieCard (many)
└── MovieDetails (shown on card click)
```

**🤔 Think About:**
- What problem does React solve that vanilla JavaScript doesn't?
- When does a component re-render? What triggers it?
- Why does React need a `key` prop when rendering lists?
- What's the difference between props and state?

**Stretch Challenges:**
- Add pagination or infinite scroll for search results
- Add a "Favorites" feature using state (no persistence needed yet)
- Add genre-based browsing
- Create a custom hook `useDebounce` for the search input

**📚 Resources to Search For:**
- "React official tutorial" (react.dev — the new docs are excellent)
- "Vite React setup tutorial"
- "useState React hook explained"
- "React conditional rendering patterns"

---

### **WEEK 8: React Intermediate — Hooks & Routing**
**🎯 Project: Multi-Page Recipe App**

**Concepts to Learn (Just-in-Time):**
- `useEffect` hook: side effects, dependency arrays, cleanup
- React Router (v6): `BrowserRouter`, `Routes`, `Route`, `Link`, `useParams`, `useNavigate`
- Custom hooks
- `useRef` hook
- Lifting state up
- Component composition patterns
- Controlled vs uncontrolled components (forms)

**Project Details:**
Build a multi-page recipe application where users can browse, search, and save recipes. Use [TheMealDB](https://www.themealdb.com/api.php) (free, no key needed) or [Spoonacular API](https://spoonacular.com/food-api).

**Requirements:**
- **Home Page (`/`):** Featured/random recipes, search bar, category filters
- **Search Results Page (`/search?q=chicken`):** Grid of matching recipes
- **Recipe Detail Page (`/recipe/:id`):** Full recipe with ingredients, instructions, image, video (if available)
- **Favorites Page (`/favorites`):** Saved recipes (persist in localStorage)
- **Categories Page (`/categories`):** Browse by cuisine or meal type
- Navigation bar present on all pages with active link highlighting
- Loading skeletons (not just spinners) while data loads
- 404 page for invalid routes
- URL-driven state: the search query should be in the URL so users can share/bookmark search links

**Custom Hooks to Create:**
- `useFetch(url)` — generic hook for data fetching with loading/error states
- `useLocalStorage(key, initialValue)` — hook that syncs state with localStorage

**🤔 Think About:**
- Why does `useEffect` need a dependency array? What happens without one?
- What's the difference between client-side routing (React Router) and traditional server-side routing?
- When should you create a custom hook vs. keeping logic in a component?
- Why do we clean up effects? What could go wrong if you don't?

**Stretch Challenges:**
- Add recipe rating system (stored locally)
- Add "recently viewed" recipes
- Implement a shopping list: click "Add ingredients to shopping list" on a recipe detail page
- Add print-friendly styles for recipes
- Add lazy loading for images

**📚 Resources to Search For:**
- "React useEffect complete guide" (Dan Abramov's blog)
- "React Router v6 tutorial"
- "Custom hooks React tutorial"
- "React loading skeleton"

---

### **WEEK 9: State Management & Tailwind in React**
**🎯 Project: E-Commerce Product Store (Frontend Only)**

**Concepts to Learn (Just-in-Time):**
- Context API: `createContext`, `useContext`, `Provider`
- `useReducer` hook for complex state logic
- State management patterns: when to use useState vs useReducer vs Context
- Tailwind CSS with React (install via Vite plugin)
- Tailwind component patterns: reusable styled components
- React performance basics: `React.memo`, understanding unnecessary re-renders

**Project Details:**
Build a frontend e-commerce store with a shopping cart. Use [Fake Store API](https://fakestoreapi.com/) or create your own mock data.

**Requirements:**
- **Product Listing Page:** Grid of products with image, name, price, rating, "Add to Cart" button
- **Product Filters:** By category, price range (slider), rating, sort by (price low-high, high-low, name)
- **Product Detail Page:** Large image, full description, reviews, quantity selector, "Add to Cart"
- **Shopping Cart (slide-out drawer or separate page):**
  - List of added items with quantity adjustors (+/-)
  - Remove item button
  - Subtotal per item and total price
  - "Clear Cart" button
- **Cart Badge:** Shows item count on the navigation cart icon
- **Cart persists** in localStorage across page reloads

**State Architecture:**
```
CartContext (useReducer)
├── state: { items: [], totalItems: 0, totalPrice: 0 }
├── actions: ADD_ITEM, REMOVE_ITEM, UPDATE_QUANTITY, CLEAR_CART
└── Provide at App level, consume in any component
```

**Style entirely with Tailwind CSS.**

**🤔 Think About:**
- When is Context API sufficient vs. when would you need something like Redux or Zustand?
- What's the difference between `useReducer` and `useState`? When would you choose one over the other?
- If you add an item to the cart from the Product Detail page, how does the Cart icon in the Navbar know to update? (This is the problem Context solves.)
- Are there any performance implications of putting everything in a single Context?

**Stretch Challenges:**
- Add a "Wishlist" feature with its own Context
- Add product comparison (select 2-3 products to compare side-by-side)
- Add a checkout flow (multi-step form: shipping → payment → review → confirmation) — frontend only
- Implement optimistic UI updates
- Add image zoom on product detail page

**📚 Resources to Search For:**
- "React Context API tutorial"
- "useReducer React tutorial"
- "Tailwind CSS with React Vite setup"
- "React shopping cart tutorial"

---

### **WEEK 10: TypeScript with React**
**🎯 Project: Project Management Board (Kanban Board)**

**Concepts to Learn (Just-in-Time):**
- TypeScript basics: types, interfaces, type aliases, unions, generics
- TypeScript with React: typing props, state, events, refs
- TypeScript with hooks: typed `useState`, `useReducer`, `useContext`
- `React.FC` vs explicit prop typing
- Drag and drop in React (use `@dnd-kit/core` library or HTML5 drag-and-drop API)

**Project Setup:**
```bash
npm create vite@latest kanban-board -- --template react-ts
```

**Project Details:**
Build a Trello-like Kanban board where users can create tasks, organize them into columns, and drag them between columns.

**Requirements:**
- **Board** with at least 3 default columns: "To Do", "In Progress", "Done"
- **Add/edit/delete columns** (custom column names)
- **Add/edit/delete task cards** within columns
- Each task card has: title, description, priority label (color-coded), due date, assigned person (avatar or initials)
- **Drag and drop** cards between columns and to reorder within a column
- **Filter tasks** by priority or assignee
- Everything persisted in localStorage
- **Fully typed with TypeScript** — no `any` types allowed

**TypeScript Requirements:**
```typescript
interface Task {
  id: string;
  title: string;
  description: string;
  priority: 'low' | 'medium' | 'high';
  dueDate: string;
  assignee: string;
  columnId: string;
  order: number;
}

interface Column {
  id: string;
  title: string;
  taskIds: string[];
}

interface Board {
  columns: Record<string, Column>;
  tasks: Record<string, Task>;
  columnOrder: string[];
}
```

**🤔 Think About:**
- How does TypeScript help you catch bugs before they happen?
- What's the difference between `interface` and `type`? When would you use each?
- How do you type an event handler in React with TypeScript?
- What's the data structure challenge of drag-and-drop? (Hint: reordering arrays efficiently)

**Stretch Challenges:**
- Add multiple boards
- Add task comments/activity log
- Add labels/tags to tasks
- Implement undo/redo functionality
- Add keyboard shortcuts (press "N" to add new task)
- Add swimlanes (horizontal grouping by assignee)

**📚 Resources to Search For:**
- "TypeScript handbook" (typescriptlang.org)
- "TypeScript with React cheatsheet" (react-typescript-cheatsheet.netlify.app)
- "dnd-kit tutorial React"
- "TypeScript generics explained"

---

### **WEEK 11: Testing & Build Tools**
**🎯 Project: Add Tests to Your Kanban Board + Build a Component Library**

**Concepts to Learn (Just-in-Time):**
- Testing philosophy: what to test, testing pyramid
- Vitest: setup, writing unit tests, describe/it/expect
- React Testing Library: render, screen, userEvent, queries
- Testing components with state, events, and async operations
- Mocking: mock functions, mock modules, mock API calls
- Build tools: what Vite does under the hood, ESBuild, bundling concepts
- ESLint and Prettier: setup, configuration, auto-formatting
- Storybook (optional but valuable): component documentation

**Project Details — Part A: Test Your Kanban Board**
Go back to your Week 10 project and add comprehensive tests.

**Testing Requirements:**
- At least 20 tests total
- Unit tests for utility functions (e.g., reordering logic, filtering)
- Component tests for:
  - TaskCard renders correctly with different props
  - Adding a new task updates the board
  - Deleting a task shows confirmation and removes it
  - Filtering tasks shows only matching results
  - Moving a task between columns updates state correctly
- Test edge cases: empty board, very long task titles, special characters

**Project Details — Part B: Reusable Component Library**
Build a small library of reusable UI components with Tailwind that you can use in future projects.

**Components to Build (with tests for each):**
- `Button` (variants: primary, secondary, danger, ghost; sizes: sm, md, lg; loading state)
- `Input` (with label, error message, helper text)
- `Modal` (open/close, overlay click to close, escape key to close)
- `Toast/Notification` (success, error, warning, info; auto-dismiss)
- `Card` (with header, body, footer slots)
- `Badge` (different colors, sizes)
- `Dropdown` (accessible, keyboard navigable)

**🤔 Think About:**
- What makes a test valuable vs. what's just testing implementation details?
- Should you test that a button has the class "bg-blue-500" or should you test that it's visible and clickable?
- How do you test something that involves async operations (API calls)?
- What's the difference between unit tests and integration tests?

**Stretch Challenges:**
- Achieve 80%+ code coverage on your Kanban board
- Add accessibility tests using jest-axe
- Document your component library with Storybook
- Add visual regression tests
- Set up a pre-commit hook with Husky that runs tests and linting before allowing a commit

**📚 Resources to Search For:**
- "Vitest getting started"
- "React Testing Library tutorial"
- "Kent C. Dodds testing best practices"
- "ESLint Prettier setup Vite React"

---

### **WEEK 12: Frontend Checkpoint Project**
**🎯 Project: Social Media Dashboard (Frontend Only)**

**Concepts to Learn (Just-in-Time):**
- Data visualization: Chart.js or Recharts library
- Advanced responsive design patterns
- Performance optimization: React.lazy, Suspense, code splitting
- Form validation library: React Hook Form + Zod (or Yup)
- Advanced Tailwind: custom themes, plugins, dark mode

**Project Details:**
Build a comprehensive social media analytics dashboard. Use mock data (create realistic JSON files) since you don't have a backend yet.

**Requirements:**
- **Authentication UI** (login/register pages — no real auth yet, just form validation and UI)
- **Dashboard Page:**
  - Summary cards: total followers, engagement rate, posts this week, new followers
  - Line chart: follower growth over 30 days
  - Bar chart: engagement by platform
  - Pie chart: audience demographics
  - Recent activity feed
- **Analytics Page:**
  - Interactive charts with date range picker
  - Platform comparison table
  - Top-performing posts list
- **Posts Page:**
  - Create/schedule new post (form with validation)
  - Post preview (shows how it would look on different platforms)
  - Post history with filters and search
- **Settings Page:**
  - Profile settings form
  - Notification preferences (toggles)
  - Connected accounts
- **Responsive sidebar** navigation (collapsible on mobile)
- **Dark/Light mode** toggle with system preference detection
- **Fully typed with TypeScript**
- **Tested**: at least 15 meaningful tests
- **Performance**: lazy-load pages/routes, optimized re-renders

**🤔 Think About:**
- How would this app change when you connect it to a real backend? What would stay the same?
- How do you handle forms with many fields and complex validation rules?
- What's the user experience of loading states for dashboard data?

**Stretch Challenges:**
- Add real-time-simulated data (use `setInterval` to simulate live updates)
- Add export to PDF/CSV functionality for reports
- Make the dashboard customizable (drag to rearrange widgets)
- Add notification system with a bell icon and dropdown
- Implement infinite scroll for the posts page

---

## 🟠 PHASE 3: BACKEND DEVELOPMENT (Weeks 13–18)

---

### **WEEK 13: Node.js & Express Fundamentals**
**🎯 Project: REST API for a Bookstore**

**Concepts to Learn (Just-in-Time):**
- Node.js: what it is, event loop basics, modules (CommonJS vs ES modules)
- Express.js: routing, middleware, request/response cycle
- REST API design: HTTP methods (GET, POST, PUT, PATCH, DELETE), status codes, resource naming
- Request handling: params, query strings, body parsing
- Middleware: built-in, third-party (cors, morgan), custom middleware
- Error handling middleware
- API testing with Postman or Thunder Client (VS Code extension)
- Project structure for Express apps
- Environment variables with `dotenv`

**Project Details:**
Build a RESTful API for a bookstore. Store data in memory (a JavaScript array) for now — you'll add a database next week.

**API Endpoints:**
```
Books:
  GET    /api/books          - List all books (with filtering, sorting, pagination)
  GET    /api/books/:id      - Get a single book
  POST   /api/books          - Add a new book
  PUT    /api/books/:id      - Update a book (full update)
  PATCH  /api/books/:id      - Partial update
  DELETE /api/books/:id      - Delete a book

Authors:
  GET    /api/authors         - List all authors
  GET    /api/authors/:id     - Get author with their books
  POST   /api/authors         - Add a new author

Categories:
  GET    /api/categories      - List all categories
  GET    /api/categories/:id/books - Get books in a category
```

**Requirements:**
- Proper HTTP status codes (200, 201, 204, 400, 404, 500)
- Request validation: reject requests with missing or invalid fields (return 400 with descriptive error messages)
- Pagination: `GET /api/books?page=2&limit=10`
- Filtering: `GET /api/books?author=tolkien&category=fantasy`
- Sorting: `GET /api/books?sort=title&order=asc`
- Search: `GET /api/books?search=ring` (search in title and description)
- Logging middleware (log every request: method, URL, status code, response time)
- Error handling middleware (centralized error handling)
- CORS configured
- Organized file structure:
```
bookstore-api/
├── src/
│   ├── routes/
│   │   ├── books.js
│   │   ├── authors.js
│   │   └── categories.js
│   ├── middleware/
│   │   ├── errorHandler.js
│   │   ├── logger.js
│   │   └── validator.js
│   ├── controllers/
│   │   └── bookController.js
│   ├── data/
│   │   └── books.js (mock data)
│   └── app.js
├── .env
├── .gitignore
└── package.json
```

**🤔 Think About:**
- What is middleware and why is it so important in Express?
- Why do we use different HTTP methods? Couldn't everything just be POST?
- What's the difference between PUT and PATCH?
- Why separate routes, controllers, and data? What happens if you put everything in one file?
- What does "RESTful" actually mean? What makes an API RESTful vs. not?

**Stretch Challenges:**
- Add rate limiting middleware
- Add request validation using Joi or Zod
- Write API documentation (manually or using Swagger/OpenAPI)
- Add a `/api/stats` endpoint that returns aggregate data (total books, books per category, etc.)
- Handle file upload for book cover images (use multer)

**📚 Resources to Search For:**
- "Express.js tutorial" (expressjs.com)
- "REST API design best practices"
- "Express middleware explained"
- "Postman API testing tutorial"
- "HTTP status codes cheatsheet"

---

### **WEEK 14: Databases — PostgreSQL**
**🎯 Project: Bookstore API with PostgreSQL**

**Concepts to Learn (Just-in-Time):**
- Relational database concepts: tables, rows, columns, schemas
- SQL fundamentals: SELECT, INSERT, UPDATE, DELETE, WHERE, JOIN, GROUP BY, ORDER BY
- Database design: primary keys, foreign keys, relationships (one-to-many, many-to-many)
- Normalization: 1NF, 2NF, 3NF (practical understanding)
- PostgreSQL: installation, psql CLI, pgAdmin (GUI)
- Node.js + PostgreSQL: using `pg` (node-postgres) library
- Connection pooling
- Database migrations: concept and basic implementation
- SQL injection and parameterized queries
- Indexing basics

**Project Details:**
Replace your in-memory bookstore data with a real PostgreSQL database.

**Database Schema Design:**
```sql
-- Design these tables yourself first, then compare with this:
CREATE TABLE authors (
  id SERIAL PRIMARY KEY,
  name VARCHAR(255) NOT NULL,
  bio TEXT,
  birth_year INTEGER,
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

CREATE TABLE categories (
  id SERIAL PRIMARY KEY,
  name VARCHAR(100) NOT NULL UNIQUE,
  description TEXT
);

CREATE TABLE books (
  id SERIAL PRIMARY KEY,
  title VARCHAR(255) NOT NULL,
  isbn VARCHAR(13) UNIQUE,
  description TEXT,
  price DECIMAL(10, 2) NOT NULL,
  author_id INTEGER REFERENCES authors(id),
  published_date DATE,
  pages INTEGER,
  cover_image_url TEXT,
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
  updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

-- Many-to-many: books can be in multiple categories
CREATE TABLE book_categories (
  book_id INTEGER REFERENCES books(id) ON DELETE CASCADE,
  category_id INTEGER REFERENCES categories(id) ON DELETE CASCADE,
  PRIMARY KEY (book_id, category_id)
);

CREATE TABLE reviews (
  id SERIAL PRIMARY KEY,
  book_id INTEGER REFERENCES books(id) ON DELETE CASCADE,
  reviewer_name VARCHAR(255) NOT NULL,
  rating INTEGER CHECK (rating >= 1 AND rating <= 5),
  comment TEXT,
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

**Requirements:**
- All existing API endpoints now use PostgreSQL instead of in-memory arrays
- Use parameterized queries (never concatenate user input into SQL!)
- Add review endpoints: `POST /api/books/:id/reviews`, `GET /api/books/:id/reviews`
- Join queries: when fetching a book, include author info and categories
- Aggregation: `GET /api/books/:id` should include average rating
- Pagination with total count: `{ data: [...], total: 150, page: 2, limit: 10, totalPages: 15 }`
- Seed script: create a script that populates the database with sample data
- Migration files: at least basic up/down SQL files for creating/dropping tables
- Database connection pooling configured
- Add indexes on frequently queried columns

**🤔 Think About:**
- Why do we use a junction table (book_categories) for many-to-many relationships?
- What is SQL injection? Try to "attack" your own API — does your parameterized query protect you?
- What's the N+1 query problem? (Example: fetching 10 books, then making 10 separate queries for each book's author)
- Why use connection pooling instead of creating a new connection for each request?

**Stretch Challenges:**
- Add full-text search using PostgreSQL's `tsvector` and `tsquery`
- Use database transactions for operations that modify multiple tables
- Add a `GET /api/statistics` endpoint with complex aggregation queries
- Create an automated backup script for your database
- Try an ORM: refactor one route to use Prisma or Drizzle and compare the experience with raw SQL

**📚 Resources to Search For:**
- "PostgreSQL tutorial for beginners"
- "SQL joins explained visually"
- "node-postgres (pg) tutorial"
- "Database normalization explained simply"
- "SQL injection explained"

---

### **WEEK 15: Authentication & Authorization**
**🎯 Project: User Authentication System for Your Bookstore**

**Concepts to Learn (Just-in-Time):**
- Authentication vs. Authorization: what's the difference?
- Password hashing: bcrypt, why we never store plain passwords
- JSON Web Tokens (JWT): structure (header.payload.signature), signing, verification
- JWT flow: access tokens, refresh tokens
- HTTP cookies vs. Authorization headers for token storage
- Protected routes: middleware that checks authentication
- Role-based access control (RBAC): user roles (admin, editor, viewer)
- Rate limiting for auth endpoints (prevent brute force)
- Input sanitization

**Project Details:**
Add a complete authentication and authorization system to your bookstore API.

**New Database Tables:**
```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  email VARCHAR(255) UNIQUE NOT NULL,
  username VARCHAR(100) UNIQUE NOT NULL,
  password_hash VARCHAR(255) NOT NULL,
  role VARCHAR(20) DEFAULT 'user' CHECK (role IN ('user', 'editor', 'admin')),
  is_active BOOLEAN DEFAULT true,
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP,
  updated_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

CREATE TABLE refresh_tokens (
  id SERIAL PRIMARY KEY,
  user_id INTEGER REFERENCES users(id) ON DELETE CASCADE,
  token VARCHAR(500) NOT NULL,
  expires_at TIMESTAMP NOT NULL,
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

**New API Endpoints:**
```
Auth:
  POST   /api/auth/register    - Create a new user account
  POST   /api/auth/login       - Login, receive access + refresh tokens
  POST   /api/auth/logout      - Invalidate refresh token
  POST   /api/auth/refresh     - Get new access token using refresh token
  GET    /api/auth/me          - Get current user profile (protected)
  PUT    /api/auth/me          - Update profile (protected)
  PUT    /api/auth/password    - Change password (protected)

Updated Book Endpoints:
  GET    /api/books            - Public (anyone can browse)
  POST   /api/books            - Protected (editor or admin only)
  PUT    /api/books/:id        - Protected (editor or admin only)
  DELETE /api/books/:id        - Protected (admin only)
  POST   /api/books/:id/reviews - Protected (any authenticated user)
```

**Requirements:**
- Password hashing with bcrypt (12+ salt rounds)
- JWT access tokens (15-minute expiry)
- JWT refresh tokens (7-day expiry, stored in database)
- `authMiddleware`: extracts and verifies JWT from `Authorization: Bearer <token>` header
- `roleMiddleware('admin')`: checks if authenticated user has the required role
- Registration validation: email format, password strength (min 8 chars, must include number and special char)
- Login rate limiting: max 5 attempts per IP in 15 minutes
- Proper error messages that don't leak information (e.g., "Invalid credentials" not "User not found" or "Wrong password")
- Reviews are now linked to authenticated users

**🤔 Think About:**
- Why use bcrypt instead of SHA-256 or MD5 for passwords?
- Why do we need both access tokens and refresh tokens? Why not just one long-lived token?
- Where should tokens be stored on the client side? (localStorage vs. httpOnly cookies — security implications)
- What happens if a JWT secret key is compromised? How would you handle it?
- Why should error messages be vague for authentication? ("Invalid credentials" vs "User not found")

**Stretch Challenges:**
- Add email verification on registration (generate a verification token, log it to console since you don't have an email service yet)
- Add "forgot password" flow (generate reset token, log it)
- Add OAuth2 login with Google (use Passport.js)
- Add account lockout after too many failed login attempts
- Add session management: users can see their active sessions and revoke them
- Add two-factor authentication (TOTP) using `otplib`

**📚 Resources to Search For:**
- "JWT authentication Node.js tutorial"
- "bcrypt password hashing Node.js"
- "Refresh token rotation explained"
- "OWASP authentication cheatsheet"
- "Express middleware for authentication"

---

### **WEEK 16: File Uploads, Email & Advanced API Features**
**🎯 Project: Complete Bookstore API with Advanced Features**

**Concepts to Learn (Just-in-Time):**
- File uploads: Multer middleware, file validation (type, size)
- Cloud storage: AWS S3 basics (or use Cloudinary — easier for beginners)
- Email sending: Nodemailer with SendGrid, Mailgun, or Mailtrap (for testing)
- API rate limiting: express-rate-limit
- Request validation: Joi or Zod for schema validation
- API documentation: Swagger/OpenAPI specification
- Caching basics: in-memory caching with node-cache
- Pagination strategies: offset vs. cursor-based
- WebHooks concept

**Project Details:**
Add production-grade features to your bookstore API.

**New Features:**
1. **Book Cover Image Upload:**
   - `POST /api/books/:id/cover` — upload image (accept jpg, png, webp; max 5MB)
   - Store images on Cloudinary (free tier) or locally in `/uploads`
   - Return image URL that can be used in the frontend
   - Generate thumbnails (if using Cloudinary, this is automatic)

2. **Email Notifications:**
   - Welcome email on registration
   - Password reset email with reset link
   - Order confirmation email (for the e-commerce expansion)
   - Use Mailtrap.io (free) for testing so you don't send real emails

3. **Advanced Querying:**
   - Cursor-based pagination for better performance
   - Complex filtering: `GET /api/books?price_min=10&price_max=50&rating_min=4`
   - Full-text search across title, description, and author name

4. **API Documentation:**
   - Add Swagger/OpenAPI documentation using `swagger-jsdoc` and `swagger-ui-express`
   - Every endpoint documented with request/response examples
   - Available at `GET /api/docs`

5. **Caching:**
   - Cache frequently requested data (popular books, categories list)
   - Cache invalidation when data changes

6. **Webhooks:**
   - `POST /api/webhooks/register` — register a webhook URL
   - When a new book is added, send a POST request to all registered webhook URLs

**Requirements:**
- Comprehensive request validation on all endpoints (use Zod)
- Rate limiting: 100 requests per 15 minutes per IP (general), 5 per 15 minutes for auth endpoints
- All new features fully tested
- API docs available at `/api/docs`
- Proper error responses with consistent format:
```json
{
  "success": false,
  "error": {
    "code": "VALIDATION_ERROR",
    "message": "Invalid input",
    "details": [
      { "field": "price", "message": "Price must be a positive number" }
    ]
  }
}
```

**🤔 Think About:**
- Why not store uploaded images directly in your database?
- What's the difference between offset pagination and cursor-based pagination? When does each shine?
- What happens if your email service is down when a user registers? Should you fail the registration?
- How do webhooks enable loose coupling between systems?

**Stretch Challenges:**
- Add image optimization (resize, compress) before storage
- Implement webhook retry logic with exponential backoff
- Add API versioning (`/api/v1/books`, `/api/v2/books`)
- Add a changelog endpoint
- Add request/response compression with gzip
- Implement ETags for caching

---

### **WEEK 17: Redis & Performance**
**🎯 Project: Add Redis Caching & Real-Time Features to Bookstore**

**Concepts to Learn (Just-in-Time):**
- Redis: what it is, data structures (strings, hashes, lists, sets, sorted sets)
- Redis use cases: caching, session storage, rate limiting, pub/sub
- Redis CLI basics: SET, GET, DEL, EXPIRE, TTL
- Using Redis with Node.js (`ioredis` or `redis` package)
- Caching strategies: cache-aside, write-through, write-behind
- Cache invalidation patterns
- WebSockets with Socket.io: real-time bidirectional communication
- Server-Sent Events (SSE)

**Project Details:**
Install Redis and add caching, session management, and real-time features.

**Redis Features to Implement:**

1. **API Response Caching:**
   - Cache `GET /api/books` results (key: query params hash, TTL: 5 minutes)
   - Cache individual book lookups (TTL: 10 minutes)
   - Invalidate cache when books are created, updated, or deleted
   - Add `X-Cache: HIT` or `X-Cache: MISS` response headers

2. **Rate Limiting with Redis:**
   - Replace in-memory rate limiting with Redis-backed rate limiting (works across multiple server instances)
   - Sliding window rate limiting

3. **Session Storage:**
   - Move refresh tokens from PostgreSQL to Redis (they're temporary data, perfect for Redis)
   - Track active sessions per user

4. **Real-Time Features with WebSockets:**
   - When a new book is added, push a notification to all connected clients
   - Live "currently browsing" count on each book
   - Real-time review updates: when someone posts a review, it appears instantly for other viewers

5. **Leaderboard:**
   - Use Redis sorted sets for "Most Popular Books" (sorted by view count)
   - `GET /api/books/popular` reads from Redis sorted set

**Performance Testing:**
- Compare response times with and without Redis caching
- Log cache hit/miss ratios
- Use `console.time()` or a proper benchmarking approach

**🤔 Think About:**
- When should you use Redis vs. PostgreSQL? What data belongs in each?
- What's the danger of stale cache? How do you balance freshness vs. performance?
- What happens if Redis goes down? Should your API also go down? (Graceful degradation)
- How is WebSocket communication different from HTTP? When would you use each?

**Stretch Challenges:**
- Implement a Redis-backed job queue for email sending (process emails asynchronously)
- Add Redis pub/sub for multi-instance communication
- Implement a simple search autocomplete using Redis sorted sets
- Add analytics: track most searched terms, most viewed books, peak usage hours
- Benchmark your API with `autocannon` or `k6` — before and after caching

**📚 Resources to Search For:**
- "Redis tutorial for beginners"
- "Redis with Node.js tutorial"
- "Socket.io React tutorial"
- "Caching strategies explained"
- "Redis data structures guide"

---

### **WEEK 18: Backend Checkpoint — Full-Stack Integration**
**🎯 Project: Connect Your React Frontend to Your Backend**

**Concepts to Learn (Just-in-Time):**
- Full-stack architecture: how frontend and backend communicate
- CORS configuration: understanding origin, methods, headers
- Environment variables in React (Vite: `VITE_` prefix)
- Axios or Fetch with interceptors for automatic token handling
- Protected routes in React (redirect unauthenticated users)
- Global error handling in frontend (API errors → user-friendly messages)
- Form submission to backend
- Image upload from frontend
- Loading/error states for every API call
- Optimistic updates

**Project Details:**
Build a complete React frontend for your bookstore API. This is your first truly full-stack application.

**Frontend Pages & Features:**
```
Public:
  /                    - Home page (featured books, categories)
  /books               - Book catalog with search, filter, sort
  /books/:id           - Book detail with reviews
  /login               - Login page
  /register            - Registration page

Protected (must be logged in):
  /profile             - User profile, edit settings
  /books/:id/review    - Write a review
  /favorites           - User's favorite books

Admin (admin role only):
  /admin/books         - CRUD books (create, edit, delete)
  /admin/books/new     - Add new book with image upload
  /admin/users         - User management
  /admin/dashboard     - Stats and analytics
```

**Technical Requirements:**
- **API Service Layer:** Create an Axios instance with:
  - Base URL from environment variable
  - Request interceptor: automatically attach JWT access token
  - Response interceptor: if 401 received, try to refresh token, then retry the original request
- **Auth Context:** Global auth state with login, logout, register, refresh capabilities
- **Protected Route Component:** Wrapper that redirects to /login if not authenticated
- **Admin Route Component:** Also checks for admin role
- **Every API call** should handle loading, success, and error states
- **Form Handling:** Use React Hook Form + Zod for all forms
- **Image Upload:** Preview before upload, progress indicator
- **Real-Time:** Connect to WebSocket for live notifications (new book added, new review)
- **Responsive** and styled with Tailwind CSS
- **TypeScript** throughout

**🤔 Think About:**
- How do you keep the frontend and backend auth in sync? What if the token expires mid-session?
- Should you store the JWT in localStorage or in a cookie? What are the security implications of each?
- What happens if the backend is down? What does the user see?
- How do you prevent stale data? (User is looking at a book that someone else deletes)

**Stretch Challenges:**
- Implement "remember me" functionality
- Add social login (Google OAuth)
- Add offline support with service workers
- Implement infinite scroll with cursor-based pagination
- Add end-to-end tests with Playwright

---

## 🔴 PHASE 4: ADVANCED (Weeks 19–24)

---

### **WEEK 19: Next.js & Server-Side Rendering**
**🎯 Project: Blog Platform with Next.js**

**Concepts to Learn (Just-in-Time):**
- Next.js App Router: file-based routing, layouts, pages, loading, error boundaries
- Server Components vs. Client Components
- SSR (Server-Side Rendering) vs. SSG (Static Site Generation) vs. ISR (Incremental Static Regeneration)
- Server Actions
- Next.js API routes
- Metadata API for SEO
- Image optimization with `next/image`
- Middleware in Next.js

**Project Details:**
Build a full-featured blog platform using Next.js. This replaces the traditional React + Express setup with a unified framework.

**Features:**
- **Public Blog:**
  - Home page with recent posts (SSG with ISR — revalidate every 10 minutes)
  - Individual post pages (SSG — generated at build time for existing posts)
  - Category/tag pages
  - Author pages
  - Search functionality
  - Comments on posts
  - SEO-optimized with dynamic meta tags, Open Graph images, structured data (JSON-LD)

- **Author Dashboard:**
  - Rich text editor for writing posts (use Tiptap or MDX)
  - Draft/publish/archive workflow
  - Post analytics (views, reading time)
  - Image management
  - Comment moderation

- **Authentication:**
  - Use NextAuth.js (Auth.js) for authentication
  - Support email/password and at least one OAuth provider (GitHub or Google)

- **Database:**
  - Use Prisma ORM with PostgreSQL
  - Define models for User, Post, Comment, Category, Tag

**🤔 Think About:**
- When should a page be server-rendered vs. statically generated vs. client-rendered?
- What's the SEO advantage of server-side rendering?
- How are Server Components different from Client Components? What goes where?
- Why would you use an ORM like Prisma instead of raw SQL?

**Stretch Challenges:**
- Add a newsletter subscription system
- Add RSS feed generation
- Add reading progress indicator
- Add "related posts" based on tags
- Add view counting that doesn't slow down page loads
- Deploy to Vercel and measure performance

**📚 Resources to Search For:**
- "Next.js 14 App Router tutorial"
- "Server Components vs Client Components"
- "NextAuth.js tutorial"
- "Prisma getting started"

---

### **WEEK 20: Docker & Containerization**
**🎯 Project: Dockerize Your Full-Stack Bookstore App**

**Concepts to Learn (Just-in-Time):**
- What is containerization? Containers vs. VMs
- Docker basics: images, containers, Dockerfile, volumes, networks
- Docker CLI: build, run, stop, exec, logs, ps
- Dockerfile best practices: layers, caching, multi-stage builds, .dockerignore
- Docker Compose: multi-container applications
- Environment variables in Docker
- Docker volumes: data persistence
- Docker networking: containers talking to each other

**Project Details:**
Containerize your entire bookstore application (React frontend, Node.js backend, PostgreSQL, Redis) using Docker.

**Files to Create:**

1. **Backend Dockerfile** (`backend/Dockerfile`):
```dockerfile
# You'll write this yourself, but here's the approach:
# 1. Use node:20-alpine as base
# 2. Set working directory
# 3. Copy package*.json first (layer caching!)
# 4. Run npm ci
# 5. Copy source code
# 6. Expose port
# 7. Set CMD
```

2. **Frontend Dockerfile** (`frontend/Dockerfile`):
   - Multi-stage build: stage 1 builds the React app, stage 2 serves it with Nginx

3. **Docker Compose** (`docker-compose.yml`):
```yaml
# Services you'll define:
# - frontend (React + Nginx)
# - backend (Node.js/Express)
# - db (PostgreSQL)
# - redis (Redis)
# - adminer (database GUI - optional but helpful)
```

**Requirements:**
- All four services start with a single `docker-compose up`
- Database data persists in a Docker volume (survives `docker-compose down`)
- Redis data persists in a Docker volume
- Backend waits for database to be ready (depends_on + healthcheck)
- Frontend proxies API requests to backend (Nginx config)
- Environment variables are properly managed (`.env` file, not hardcoded in Dockerfile)
- `.dockerignore` files to prevent copying unnecessary files
- Multi-stage builds for production images
- Backend hot-reloading in development (bind mount source code)

**Development vs. Production:**
Create two compose files:
- `docker-compose.dev.yml` — bind mounts, hot reload, debug ports exposed
- `docker-compose.prod.yml` — optimized builds, no source code mounted

**🤔 Think About:**
- Why is the order of instructions in a Dockerfile important? (Layer caching)
- Why copy `package.json` separately before the rest of the code?
- What's the difference between `CMD` and `ENTRYPOINT`?
- How do containers in the same Docker network communicate?
- What data should and shouldn't be in Docker volumes?

**Stretch Challenges:**
- Add Nginx as a reverse proxy (frontend + backend behind single entry point)
- Add health checks for all services
- Reduce image sizes (compare before/after with multi-stage builds)
- Set up a local Docker registry
- Add log aggregation with a centralized logging container
- Create a Makefile with shortcuts: `make dev`, `make prod`, `make test`, `make clean`

**📚 Resources to Search For:**
- "Docker tutorial for beginners"
- "Dockerfile best practices"
- "Docker Compose tutorial"
- "Multi-stage Docker builds"
- "Dockerize Node.js application"

---

### **WEEK 21: Testing Strategy & CI/CD**
**🎯 Project: Comprehensive Testing + GitHub Actions Pipeline**

**Concepts to Learn (Just-in-Time):**
- Testing pyramid: unit → integration → end-to-end
- Backend testing: Supertest for API testing, test database setup/teardown
- Database testing: test fixtures, seeding, transaction rollback strategy
- End-to-end testing: Playwright (browser automation)
- CI/CD concepts: continuous integration, continuous delivery, pipelines
- GitHub Actions: workflows, jobs, steps, triggers, secrets, environment variables
- Code coverage: measurement and reporting
- Pre-commit hooks: Husky + lint-staged

**Project Details:**
Add comprehensive testing across your full-stack bookstore and set up an automated CI/CD pipeline.

**Testing Requirements:**

**Backend Tests (Vitest + Supertest):**
- Unit tests for utility functions, validators, helpers (15+ tests)
- Integration tests for API endpoints:
  - Test full CRUD flow for books
  - Test authentication flow (register → login → access protected route → refresh token → logout)
  - Test authorization (user can't access admin endpoints)
  - Test file upload
  - Test pagination, filtering, search
  - Test error cases (invalid data, not found, unauthorized)
- Use a separate test database (create/migrate before tests, drop after)
- 25+ integration tests

**Frontend Tests (Vitest + React Testing Library):**
- Component tests for key components (10+ tests)
- Hook tests for custom hooks
- Page-level integration tests

**End-to-End Tests (Playwright):**
- User registration flow
- Login → browse books → add to favorites → write review
- Admin: login → add new book → verify it appears in catalog
- 5+ E2E tests

**GitHub Actions Pipeline:**
```yaml
# .github/workflows/ci.yml
name: CI Pipeline
on:
  push:
    branches: [main, develop]
  pull_request:
    branches: [main]

jobs:
  lint:
    # Run ESLint and Prettier check
  
  test-backend:
    # Set up PostgreSQL and Redis services
    # Run backend tests
    # Upload coverage report
  
  test-frontend:
    # Run frontend tests
    # Upload coverage report
  
  e2e:
    # Build Docker containers
    # Run Playwright tests
    # Upload test artifacts (screenshots, videos)
  
  build:
    # Build Docker images
    # Push to container registry (if all tests pass)
```

**Requirements:**
- All tests pass in CI
- Code coverage > 70% for backend, > 60% for frontend
- Pipeline fails if any test fails, if linting fails, or if TypeScript has errors
- Successful build creates Docker images
- Branch protection: main branch requires CI to pass before merge

**🤔 Think About:**
- What's the right balance between test coverage and development speed?
- Should you test implementation details or behavior?
- How do you test database interactions without affecting production data?
- What should trigger a CI pipeline? Every push? Only PRs?

**Stretch Challenges:**
- Add visual regression testing with Playwright screenshots
- Add performance testing in CI (Lighthouse CI)
- Set up automated dependency updates (Renovate or Dependabot)
- Add changelog generation from commit messages (Conventional Commits)
- Add parallel test execution to speed up CI
- Add Slack/Discord notifications for pipeline results

---

### **WEEK 22: Cloud Deployment (AWS)**
**🎯 Project: Deploy Bookstore to AWS**

**Concepts to Learn (Just-in-Time):**
- Linux basics: navigation, file management, permissions, systemd, SSH
- AWS core services:
  - EC2: virtual servers
  - RDS: managed PostgreSQL
  - S3: file storage (book cover images)
  - ElastiCache: managed Redis (or install Redis on EC2)
  - Route 53: DNS management
  - VPC: networking fundamentals
  - IAM: users, roles, policies
  - SES: email sending (or use free tier of SendGrid)
- Domain registration and DNS configuration
- SSL/TLS certificates (Let's Encrypt or AWS Certificate Manager)
- Nginx as reverse proxy in production
- Process management: PM2 for Node.js
- Basic server security: firewall (ufw), SSH key authentication, fail2ban

**Project Details:**
Deploy your full-stack bookstore application to AWS so it's publicly accessible.

**Architecture:**
```
Internet
    │
    ▼
[Route 53 (DNS)] → [EC2 Instance]
                        │
                        ├── Nginx (reverse proxy, SSL termination)
                        │     ├── / → React frontend (static files)
                        │     └── /api → Node.js backend (PM2)
                        │
                        ├── [RDS PostgreSQL]
                        ├── [Redis (on EC2 or ElastiCache)]
                        └── [S3 Bucket (book covers)]
```

**Step-by-Step Deployment:**

1. **Set up AWS account** (use free tier!)
2. **Launch EC2 instance** (t2.micro, Ubuntu 22.04)
3. **SSH into your instance** and install: Node.js, Nginx, PM2, Redis
4. **Set up RDS PostgreSQL** instance (db.t3.micro, free tier)
5. **Create S3 bucket** for image storage
6. **Configure security groups** (firewall rules):
   - EC2: allow 80 (HTTP), 443 (HTTPS), 22 (SSH from your IP only)
   - RDS: allow 5432 only from EC2's security group
7. **Clone your repo** to EC2, install dependencies, build frontend
8. **Configure environment variables** on the server
9. **Run database migrations**
10. **Start backend with PM2**: `pm2 start src/app.js --name bookstore-api`
11. **Configure Nginx**: serve frontend static files + proxy `/api` to Node.js
12. **Set up SSL** with Let's Encrypt (Certbot)
13. **Set up a domain** (or use the EC2 public IP for now)

**Update GitHub Actions:**
Add a deployment job that:
- SSHs into your EC2 instance
- Pulls the latest code
- Installs dependencies
- Runs migrations
- Restarts the backend
- (This is a simple deployment — you'll do better in Week 23)

**🤔 Think About:**
- What's the difference between vertical and horizontal scaling?
- What happens if your EC2 instance goes down? How could you make this more resilient?
- Why put the database in a managed service (RDS) instead of on the EC2 instance?
- What's the benefit of using Nginx in front of Node.js?

**Stretch Challenges:**
- Set up a staging environment (separate EC2 instance)
- Add CloudWatch monitoring and alarms
- Set up automated database backups
- Add a CDN (CloudFront) for static assets
- Set up log rotation
- Create an AMI (snapshot) of your configured server

**📚 Resources to Search For:**
- "Deploy Node.js app to AWS EC2 tutorial"
- "AWS free tier guide"
- "Nginx reverse proxy Node.js"
- "Let's Encrypt SSL Certbot tutorial"
- "PM2 Node.js production"

---

### **WEEK 23: Infrastructure as Code & Configuration Management**
**🎯 Project: Automate Your Infrastructure with Terraform & Ansible**

**Concepts to Learn (Just-in-Time):**
- Infrastructure as Code (IaC): what and why
- Terraform basics: providers, resources, variables, outputs, state
- Terraform AWS provider: define EC2, RDS, S3, security groups in code
- Ansible basics: inventory, playbooks, roles, tasks, handlers
- Ansible for server configuration: install packages, copy files, manage services
- Immutable vs mutable infrastructure
- Terraform state management

**Project Details:**
Replace all the manual AWS setup from Week 22 with automated scripts.

**Part A: Terraform — Define Infrastructure**
```
terraform/
├── main.tf           # Provider configuration
├── variables.tf      # Input variables
├── outputs.tf        # Output values (IPs, URLs)
├── vpc.tf            # VPC, subnets, internet gateway
├── security.tf       # Security groups
├── ec2.tf            # EC2 instance
├── rds.tf            # PostgreSQL database
├── s3.tf             # S3 bucket for uploads
├── terraform.tfvars  # Variable values (gitignored!)
```

Running `terraform apply` should create your entire AWS infrastructure from scratch.

**Part B: Ansible — Configure Servers**
```
ansible/
├── inventory.yml
├── playbook.yml
└── roles/
    ├── common/         # Basic packages, firewall, SSH config
    ├── nodejs/         # Install Node.js, PM2
    ├── nginx/          # Install Nginx, configure reverse proxy, SSL
    ├── redis/          # Install and configure Redis
    └── app/            # Deploy application code
```

Running `ansible-playbook playbook.yml` should configure a fresh EC2 instance to run your app.

**🤔 Think About:**
- Why define infrastructure in code instead of clicking in the AWS console?
- What happens if you run `terraform apply` twice? (Idempotency)
- How does Terraform know what currently exists in AWS? (State file)
- What's the difference between Terraform and Ansible? When would you use each?

**Stretch Challenges:**
- Add a load balancer with Terraform
- Create separate Terraform workspaces for staging and production
- Use Ansible Vault to encrypt sensitive variables
- Add a Terraform module for reusable infrastructure components
- Integrate Terraform and Ansible into your GitHub Actions pipeline

---

### **WEEK 24: Monitoring, Logging & Observability**
**🎯 Project: Add Monitoring Stack to Your Deployed Application**

**Concepts to Learn (Just-in-Time):**
- Observability pillars: metrics, logs, traces
- Application metrics: response times, error rates, throughput, saturation
- Infrastructure metrics: CPU, memory, disk, network
- Structured logging: JSON logs, log levels, correlation IDs
- Monitoring tools: Prometheus (metrics), Grafana (visualization)
- Log management: centralized logging concepts
- Alerting: setting thresholds, notification channels
- Health checks and uptime monitoring
- Error tracking: Sentry

**Project Details:**
Add a complete monitoring and observability stack to your deployed bookstore application.

**Components to Set Up:**

1. **Structured Logging (Application):**
   - Replace `console.log` with Winston or Pino logger
   - Log format: JSON with timestamp, level, message, request ID, user ID
   - Log levels: error, warn, info, debug
   - Add a unique request ID to every API request (correlation ID)
   - Log all API requests, responses, and errors

2. **Application Metrics:**
   - Add `prom-client` to your Node.js app
   - Expose metrics at `GET /metrics`
   - Track: request count, request duration histogram, active connections, error count by type

3. **Prometheus + Grafana (Docker Compose):**
   - Add Prometheus container that scrapes your app's `/metrics` endpoint
   - Add Grafana container with dashboards:
     - API performance dashboard (request rate, latency percentiles, error rate)
     - System dashboard (CPU, memory from Node.js process metrics)
     - Business dashboard (new users, books added, reviews posted)

4. **Error Tracking:**
   - Set up Sentry (free tier) for both frontend and backend
   - Capture unhandled exceptions, rejected promises
   - Add user context to errors (who was logged in?)
   - Set up source maps for meaningful stack traces

5. **Health Checks:**
   - `GET /api/health` — returns status of all dependencies (database, Redis)
   - Set up uptime monitoring (UptimeRobot or similar free service)

6. **Alerting:**
   - Set up alerts for: error rate > 5%, response time > 2s, service down
   - Send alerts to email or Discord/Slack webhook

**🤔 Think About:**
- What's the difference between monitoring and observability?
- How do you debug a production issue if you only have logs? If you only have metrics?
- What should you alert on? How do you avoid alert fatigue?
- What are the performance implications of logging and metrics collection?

**Stretch Challenges:**
- Add distributed tracing (OpenTelemetry)
- Create a custom Grafana dashboard that tells a story about your application's health
- Set up log-based alerting (alert when specific error patterns appear)
- Add synthetic monitoring (automated checks that simulate user actions)
- Create a runbook document for common incidents

---

## ⚫ PHASE 5: CAPSTONE (Weeks 25–26)

---

### **WEEKS 25–26: Capstone Project**
**🎯 Project: Build a Production-Ready SaaS Application**

Choose ONE of the following projects and build it end-to-end:

---

#### **Option A: Project Management Tool (like Linear/Jira)**
**Features:**
- Team workspaces with invite system
- Project boards with customizable workflows (Kanban columns)
- Issues with rich text descriptions, labels, priorities, assignees, due dates
- Sprint planning: create sprints, assign issues, track progress
- Activity timeline on each issue
- Real-time updates (WebSocket): see changes others make live
- Notifications system
- Dashboard with burndown charts, velocity metrics
- Markdown support for descriptions and comments
- File attachments
- Search with filters across all issues
- Email notifications for assignments and mentions

---

#### **Option B: E-Learning Platform (like Udemy)**
**Features:**
- Instructor and student roles
- Course creation with chapters and lessons
- Video upload and streaming (use Cloudinary or AWS S3 + CloudFront)
- Rich text lesson content with code blocks
- Course progress tracking
- Quizzes per chapter with auto-grading
- Certificate generation on completion (PDF)
- Course reviews and ratings
- Instructor dashboard with enrollment analytics
- Student dashboard with enrolled courses and progress
- Search and browse courses by category
- Payment integration (Stripe test mode) for paid courses

---

#### **Option C: Real-Time Collaboration Tool (like Notion)**
**Features:**
- Workspace with pages and sub-pages (tree structure)
- Block-based editor (paragraphs, headings, lists, code, images, tables)
- Real-time collaborative editing (multiple users editing the same page)
- Page sharing with granular permissions (view, edit, admin)
- Comments and mentions
- Version history (view and restore previous versions)
- Templates library
- Full-text search across all pages
- Trash and restore
- Export to PDF/Markdown
- Dark mode

---

**Technical Requirements (All Options):**
- **Frontend:** Next.js with TypeScript, Tailwind CSS
- **Backend:** Node.js/Express API or Next.js API routes, PostgreSQL, Redis
- **Auth:** NextAuth.js with email + OAuth
- **ORM:** Prisma
- **Real-Time:** WebSockets (Socket.io) or Server-Sent Events
- **File Storage:** AWS S3 or Cloudinary
- **Testing:** Unit + Integration + at least 5 E2E tests
- **Containerized:** Docker Compose for local development
- **CI/CD:** GitHub Actions pipeline (lint → test → build → deploy)
- **Deployed:** Live on AWS or Vercel + Railway/Supabase
- **Monitored:** Basic monitoring and error tracking (Sentry)
- **Documented:**
  - README with setup instructions, architecture diagram, screenshots
  - API documentation
  - Contributing guide

**Week 25 Plan:**
- Day 1–2: System design, database schema, architecture decisions
- Day 3–4: Set up project scaffolding, Docker, database, auth
- Day 5–7: Build core features (the main functionality)

**Week 26 Plan:**
- Day 1–3: Complete features, add real-time updates, polish UI
- Day 4–5: Testing, bug fixes, performance optimization
- Day 6: Deploy, set up monitoring
- Day 7: Documentation, README, record a demo video

---

## 📊 Post-Plan: What to Do Next

After completing this 26-week plan, you'll have:
- **8+ projects** in your portfolio, from simple to production-grade
- **A deployed SaaS application** demonstrating full-stack mastery
- **Proficiency in:** HTML, CSS, Tailwind, JavaScript, TypeScript, React, Next.js, Node.js, Express, PostgreSQL, Redis, Docker, AWS, GitHub Actions, Terraform, Ansible, testing, monitoring
- **A professional GitHub** with consistent commit history

**Suggested Next Steps:**
1. **Deepen expertise** in areas that interest you most (frontend frameworks, system design, DevOps, mobile)
2. **Learn system design** patterns (load balancers, message queues, microservices, event-driven architecture)
3. **Contribute to open source** — find projects you use and start with documentation, then small bug fixes
4. **Build in public** — share your journey on Twitter/LinkedIn, write blog posts about what you learned
5. **Explore additional technologies:** GraphQL, Kubernetes, message brokers (RabbitMQ/Kafka), microservices, serverless (AWS Lambda)
6. **Study for interviews:** LeetCode for algorithms, system design practice, behavioral questions

---

## 📝 Daily Routine Template

```
Morning (1 hour):
  - Learn the concept you need for today's build step
  - Read docs, watch one tutorial, take notes

Afternoon/Main Block (2-3 hours):
  - Code! Build the project
  - When stuck: try for 20 min → search → try for 20 more min → ask for help

Evening (30 min):
  - Git commit with a meaningful message
  - Write a short note about what you learned and what was hard
  - Plan tomorrow's task
```

---

**Remember:** The goal is not to build perfect projects. The goal is to **build, struggle, learn, and ship**. Every bug you encounter is a lesson. Every error message is a teacher. Ship imperfect projects and iterate — that's how professional developers work.

**Good luck! 🚀**
