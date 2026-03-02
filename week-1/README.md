# 📅 Week 1: Detailed Daily Study Plan
## **The Internet & Your First Webpage**

**Weekly Goal:** Understand how the internet works and build a complete "About Me" webpage using only HTML.

**Total Time This Week:** ~15–20 hours

---

## 🔵 Day 1 (Monday) — Understanding the Internet & Setting Up Your Tools
**Time: ~2.5 hours**

### Morning — Learn (1 hour)
**Goal:** Understand what happens when you type a URL into your browser.

1. **Watch:** Search YouTube for *"How the internet works in 5 minutes"* — watch it twice. First time just absorb, second time take notes.
2. **Read:** Search *"MDN How does the internet work"* — read the full article slowly.
3. **In your own words, write answers to these questions in a notebook or text file:**
   - What is a client? What is a server?
   - What does HTTP stand for, and what does it do?
   - What is an IP address? What is DNS?
   - When you type `google.com` in your browser, what are the steps that happen before the page appears?

> 💡 **Don't memorize** — aim to *explain it like you're teaching a friend*. If you can't explain it simply, re-read the parts you're confused about.

### Afternoon — Set Up & Explore (1.5 hours)
**Goal:** Install your tools and understand what a code editor does.

1. **Download and install VS Code** from [code.visualstudio.com](https://code.visualstudio.com)
2. **Install these VS Code extensions** (click the Extensions icon on the left sidebar, or press `Ctrl+Shift+X`):
   - **Live Server** — lets you see changes in real-time (search "Live Server" by Ritwick Dey)
   - **Prettier** — auto-formats your code (search "Prettier - Code formatter")
   - **Auto Rename Tag** — when you rename an HTML opening tag, it renames the closing tag too
3. **Create your project:**
   - Create a new folder on your computer called `about-me`
   - Open VS Code → File → Open Folder → select `about-me`
   - Inside VS Code, create a new file: `index.html`
4. **Generate your first HTML template:**
   - In `index.html`, type `!` (exclamation mark) and press `Tab`
   - VS Code will generate a basic HTML structure — **don't panic if it looks unfamiliar!**
5. **See it in your browser:**
   - Right-click on `index.html` in VS Code → click "Open with Live Server"
   - You should see a blank white page — this is your first webpage!
6. **Experiment:** Between the `<body>` and `</body>` tags, type `Hello, World!` and save. Watch it appear in your browser.

### Evening — Reflect (15 minutes)
- Write down: *"What did I learn today? What confused me?"*
- Plan for tomorrow: *"Tomorrow I'll learn what HTML tags are and start building the page structure."*

---

## 🔵 Day 2 (Tuesday) — HTML Basics: Structure, Headings, Paragraphs, and Images
**Time: ~3 hours**

### Morning — Learn (1 hour)
**Goal:** Understand HTML elements, tags, and attributes.

1. **Read:** Search *"MDN Getting started with HTML"* — read through the article.
2. **Key concepts to understand (write notes on each):**
   - What is an HTML **element**? (opening tag + content + closing tag)
   - What is an **attribute**? (extra info inside the opening tag, like `src`, `href`, `alt`)
   - What is the difference between **block** elements and **inline** elements?
   - What goes in `<head>` vs `<body>`?
3. **Study these specific tags** (search "MDN" + the tag name for each):
   - `<h1>` through `<h6>` — headings
   - `<p>` — paragraphs
   - `<img>` — images (note: this is a **self-closing** tag)
   - `<a>` — links
   - `<br>` — line break
   - `<strong>` and `<em>` — bold and italic

### Afternoon — Build (1.5 hours)
**Goal:** Start building the top section of your About Me page.

**Step by step:**

1. **Set up the document title.** Inside `<head>`, find the `<title>` tag and change it:
   ```html
   <title>About Me - [Your Name]</title>
   ```

2. **Add a heading with your name.** Inside `<body>`:
   ```html
   <h1>Your Name Here</h1>
   ```
   Save and check your browser. You should see your name as a big heading.

3. **Add a subtitle:**
   ```html
   <h2>Aspiring Web Developer</h2>
   ```

4. **Add a paragraph about yourself.** Write 3–4 sentences:
   ```html
   <p>Hi! My name is [Name]. I'm currently learning web development. 
   I'm excited to build my first webpage and start this journey.</p>
   ```

5. **Add an image.** Find any image you'd like to use (a photo of yourself, a pet, or download a free one from [unsplash.com](https://unsplash.com)):
   - Save the image in your `about-me` folder (e.g., name it `photo.jpg`)
   - Add it to your HTML:
   ```html
   <img src="photo.jpg" alt="A description of the image" width="300">
   ```
   - **If the image doesn't appear:** Check that the filename matches exactly (case-sensitive!). Check that the image file is in the same folder as `index.html`.

6. **Add a link:**
   ```html
   <p>Here is a website I like: <a href="https://www.example.com">Example</a></p>
   ```

> 🧪 **Challenge yourself:** After each step, save and refresh. Try to predict what you'll see before you look. Did it match your expectation? If not, figure out why.

### Evening — Reflect (30 minutes)
- Look at your page so far. It's ugly and unstyled — **that's completely fine!** This week is HTML only.
- **Self-test:** Without looking at your code, can you explain what `<img src="photo.jpg" alt="my photo">` means? What does `src` do? What does `alt` do? Why is `alt` important?
- Write down one thing that surprised you.

---

## 🔵 Day 3 (Wednesday) — Lists, Tables, and Semantic HTML
**Time: ~3 hours**

### Morning — Learn (1 hour)
**Goal:** Learn about lists, tables, and why semantic HTML matters.

1. **Read about lists** (search "MDN HTML lists"):
   - `<ul>` — unordered list (bullet points)
   - `<ol>` — ordered list (numbered)
   - `<li>` — list item (goes inside `<ul>` or `<ol>`)

2. **Read about tables** (search "MDN HTML table basics"):
   - `<table>` — table container
   - `<thead>` and `<tbody>` — table sections
   - `<tr>` — table row
   - `<th>` — table header cell
   - `<td>` — table data cell

3. **Read about semantic HTML** (search "MDN HTML elements reference" and look at the "Content sectioning" section):
   - `<header>` — introductory content or navigation
   - `<nav>` — navigation links
   - `<main>` — main content of the page
   - `<section>` — a thematic grouping of content
   - `<article>` — self-contained content
   - `<footer>` — footer of the page

4. **Think about this (write your answer):**
   - *What's the difference between `<div>` and `<section>`?*
   
   > Hint: `<div>` is a generic container with no meaning. `<section>` tells the browser (and screen readers) "this is a distinct section of content." Think of it like this: `<div>` is a plain cardboard box, `<section>` is a labeled filing folder.

### Afternoon — Build (1.5 hours)
**Goal:** Add lists, a table, and reorganize your page with semantic tags.

**Step by step:**

1. **Add a hobbies list** (unordered list with 5 hobbies):
   ```html
   <h2>My Hobbies</h2>
   <ul>
     <li>Reading</li>
     <li>Hiking</li>
     <li>Cooking</li>
     <li>Photography</li>
     <li>Gaming</li>
   </ul>
   ```

2. **Add an education/experience list** (ordered list):
   ```html
   <h2>My Education</h2>
   <ol>
     <li>High School - [School Name] (2015-2019)</li>
     <li>Bachelor's Degree - [University] (2019-2023)</li>
     <li>Self-taught Web Development (2024-present)</li>
   </ol>
   ```

3. **Add a weekly schedule table:**
   ```html
   <h2>My Weekly Schedule</h2>
   <table>
     <thead>
       <tr>
         <th>Day</th>
         <th>Morning</th>
         <th>Afternoon</th>
         <th>Evening</th>
       </tr>
     </thead>
     <tbody>
       <tr>
         <td>Monday</td>
         <td>Study HTML</td>
         <td>Practice coding</td>
         <td>Exercise</td>
       </tr>
       <tr>
         <td>Tuesday</td>
         <td>Study HTML</td>
         <td>Build project</td>
         <td>Read</td>
       </tr>
     </tbody>
   </table>
   ```
   Add at least 5 rows (days).

4. **Now wrap everything in semantic tags.** Restructure your entire page like this:
   ```html
   <body>
     <header>
       <h1>Your Name</h1>
       <h2>Aspiring Web Developer</h2>
     </header>

     <main>
       <section>
         <h2>About Me</h2>
         <p>Your paragraph...</p>
         <img src="photo.jpg" alt="...">
       </section>

       <section>
         <h2>My Hobbies</h2>
         <ul>...</ul>
       </section>

       <section>
         <h2>My Education</h2>
         <ol>...</ol>
       </section>

       <section>
         <h2>My Weekly Schedule</h2>
         <table>...</table>
       </section>
     </main>

     <footer>
       <p>&copy; 2024 Your Name</p>
     </footer>
   </body>
   ```

> 🧪 **Challenge:** Try building the table from memory without looking at the example above. Get it wrong. Debug it. This is how you learn.

### Evening — Reflect (30 minutes)
- **Self-test:** Close your code. On paper, draw the nesting structure of an HTML table. (Which tag goes inside which?)
- **Think about:** Why does the table look so plain? (Because we have no CSS — but notice the browser still shows rows and columns. The HTML *structure* is there.)

---

## 🔵 Day 4 (Thursday) — Navigation, Links, and the Contact Form
**Time: ~3 hours**

### Morning — Learn (1 hour)
**Goal:** Learn about navigation, anchor links, and HTML forms.

1. **Anchor links (in-page navigation):**
   - You can link to any element on the same page using `id` attributes
   - Example: `<a href="#hobbies">Go to Hobbies</a>` will scroll to whatever element has `id="hobbies"`
   - Search "MDN creating a hyperlink" and read the section about document fragments

2. **HTML Forms** (search "MDN Your first form"):
   - `<form>` — container for form elements
   - `<label>` — text label for an input (important for accessibility!)
   - `<input>` — text input, email input, etc.
   - `<textarea>` — multi-line text input
   - `<button>` — submit button
   - Key attributes: `type`, `name`, `id`, `placeholder`, `required`

3. **Write down:**
   - What is the `for` attribute on a `<label>` and why does it matter?
   - What is the difference between `<input type="text">` and `<input type="email">`?

### Afternoon — Build (1.5 hours)
**Goal:** Add navigation and a contact form to your page.

**Step by step:**

1. **Add `id` attributes to each section:**
   ```html
   <section id="about">
     <h2>About Me</h2>
     ...
   </section>

   <section id="hobbies">
     <h2>My Hobbies</h2>
     ...
   </section>
   ```
   Do this for every section (about, hobbies, education, schedule, contact).

2. **Add a navigation bar** inside your `<header>`, after the headings:
   ```html
   <nav>
     <a href="#about">About</a>
     <a href="#hobbies">Hobbies</a>
     <a href="#education">Education</a>
     <a href="#schedule">Schedule</a>
     <a href="#contact">Contact</a>
   </nav>
   ```
   Click each link — it should scroll to that section!

3. **Add a contact section with a form:**
   ```html
   <section id="contact">
     <h2>Contact Me</h2>
     <form>
       <div>
         <label for="name">Your Name:</label>
         <input type="text" id="name" name="name" placeholder="John Doe" required>
       </div>

       <div>
         <label for="email">Your Email:</label>
         <input type="email" id="email" name="email" placeholder="john@example.com" required>
       </div>

       <div>
         <label for="message">Your Message:</label>
         <textarea id="message" name="message" rows="5" placeholder="Write your message here..." required></textarea>
       </div>

       <button type="submit">Send Message</button>
     </form>
   </section>
   ```

4. **Test the form:**
   - Try clicking "Send Message" without filling in fields — the `required` attribute should show a browser warning
   - Try entering an invalid email — `type="email"` provides basic validation
   - Note: The form **won't actually send anywhere** — that's fine! We'd need JavaScript and a backend for that.

> 🧪 **Challenge:** What happens if you remove the `for="name"` from a label and click on the label text? Now add it back and click the label text again. What's different? (The `for` attribute connects the label to the input — clicking the label focuses the input.)

### Evening — Reflect (30 minutes)
- Click through every navigation link. Does each one work?
- **Think about:** What happens when you open your HTML file by double-clicking it? Is a web server involved? 
  > Answer: **No!** Your browser is reading the file directly from your filesystem using the `file://` protocol, not `http://`. No server is involved. This is different from how real websites work.

---

## 🔵 Day 5 (Friday) — Polish, Stretch Challenges, and Deep Thinking
**Time: ~3 hours**

### Morning — Review and Fix (1 hour)
**Goal:** Review everything you've built and fix any issues.

1. **Open your page and review it section by section:**
   - Does every section have a proper heading?
   - Is the navigation working for all links?
   - Does the image display correctly?
   - Does the table have proper headers?
   - Does the form validate properly?

2. **Check your code structure:**
   - Is your code properly indented? (Select all code → right-click → Format Document, or `Shift+Alt+F`)
   - Are all tags properly closed? (Every `<div>` has a `</div>`, etc.)
   - Is your nesting correct? (No tags overlapping incorrectly)

3. **Add anything you missed from the requirements:**
   - ✅ `<!DOCTYPE html>` declaration
   - ✅ Proper `<html>`, `<head>`, `<body>` structure
   - ✅ Heading with your name
   - ✅ Paragraph about yourself
   - ✅ An image
   - ✅ Unordered list of 5 hobbies
   - ✅ Ordered list of education/experience
   - ✅ Table with weekly schedule
   - ✅ Navigation with anchor links
   - ✅ Contact form
   - ✅ Semantic tags: `<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`

### Afternoon — Stretch Challenges (1.5 hours)
**Goal:** Push yourself with features you haven't been taught explicitly.

1. **Add a FAQ section using `<details>` and `<summary>`:**
   - Search "MDN details element" — read how it works
   - **Try to figure it out yourself before looking at examples**
   - Create at least 3 FAQ items:
   ```html
   <section id="faq">
     <h2>Frequently Asked Questions</h2>
     <details>
       <summary>Why are you learning web development?</summary>
       <p>Because I want to build things that people can use on the internet!</p>
     </details>
     <!-- Add more... -->
   </details>
   ```

2. **Add `<meta>` tags in the `<head>`:**
   - Search "MDN meta element"
   - Add a description meta tag:
     ```html
     <meta name="description" content="Personal About Me page for [Your Name]">
     ```
   - Check that you already have the viewport meta tag (the `!` template usually includes it):
     ```html
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     ```
   - **Think:** Why does the viewport meta tag matter? (Hint: try viewing your page on a phone without it vs with it)

3. **Validate your HTML:**
   - Go to [validator.w3.org](https://validator.w3.org/#validate_by_input)
   - Click "Validate by Direct Input"
   - Copy-paste your entire HTML code
   - Click "Check"
   - **Fix any errors it reports.** Read each error message carefully — it tells you exactly what's wrong and on which line.

> 🧪 **Real challenge:** The validator will likely find issues you didn't expect. **Don't be discouraged** — even experienced developers get validation errors. Each fix is a learning moment.

### Evening — Deep Thinking & Reflection (30 minutes)

Answer these questions **in writing** (in a journal, notes app, or a `notes.md` file in your project):

1. **What's the difference between `<div>` and `<section>`?** Write your answer in your own words.

2. **Why does semantic HTML matter?** Think about:
   - A blind person using a screen reader to navigate your page
   - A search engine (Google) trying to understand your page
   - Another developer reading your code

3. **What happens when you open your HTML file in the browser?** Draw or describe the process:
   - Is a DNS lookup involved? (No — it's a local file)
   - Is HTTP involved? (No — it's `file://` protocol)
   - How would this be different if the page were hosted on a real server?

---

## 🔵 Day 6 (Saturday) — Exploration & Enhancement
**Time: ~2.5 hours**

### Morning — Explore What You Don't Know (1 hour)
**Goal:** Discover HTML elements you haven't used yet and explore independently.

1. **Go to MDN's HTML Element Reference:** Search "MDN HTML elements reference"
2. **Browse through the categories.** Find 3 elements you haven't used yet and try adding them to your page. Suggestions to explore:
   - `<blockquote>` — add a favorite quote
   - `<abbr>` — use it for an abbreviation (like HTML itself!)
   - `<time>` — mark up a date
   - `<address>` — your contact info in the footer
   - `<figure>` and `<figcaption>` — wrap your image with a caption
   - `<mark>` — highlight text
   - `<code>` — display code snippets

3. **For each element:**
   - Read the MDN page for it
   - Try to use it **before** looking at examples
   - Add it to your page
   - Check the result in your browser

> This exercise builds a crucial developer skill: **reading documentation and experimenting independently.**

### Afternoon — Make It Your Own (1 hour)
**Goal:** Add personal touches that go beyond the requirements.

Ideas:
- Add more content — make this genuinely *about you*
- Add a "Goals for 2024" section
- Add a "Favorite Books/Movies/Music" section with lists
- Add more rows to your schedule table
- Add an "external links" section with links to things you like
- Add a second page! (Create `hobbies.html` and link to it from your main page with `<a href="hobbies.html">`)

### Evening — Review (30 minutes)
- Read through your entire HTML file from top to bottom
- **Can you explain every single tag to someone?** If you encounter one you're unsure about, look it up
- Count how many different HTML elements you've used — try to get to 25+

---

## 🔵 Day 7 (Sunday) — Final Review, Reflection, and Planning Ahead
**Time: ~2 hours**

### Final Review (1 hour)

1. **Open your finished page** and go through it like a user would:
   - Read every section
   - Click every link
   - Try the form
   - Check how it looks if you resize the browser window really narrow

2. **Run the validator one more time.** Fix any remaining errors.

3. **Look at your code quality:**
   - Is it consistently indented?
   - Do you have comments explaining sections? Try adding a few:
     ```html
     <!-- Navigation Section -->
     <nav>
       ...
     </nav>

     <!-- Main Content -->
     <main>
       ...
     </main>
     ```

4. **Final file check — your `about-me` folder should contain:**
   - `index.html` (your main page)
   - Your image file(s)
   - Optionally: `notes.md` with your learning notes

### Weekly Reflection (30 minutes)

Write answers to these questions:

1. **What are the 3 most important things I learned this week?**
2. **What was the hardest part? How did I get through it?**
3. **What's one thing I'm still confused about?** (Write it down — it might get answered next week, or you can research it)
4. **What am I most proud of building?**

### Look Ahead (30 minutes)

1. **Read the Week 2 overview** from the learning plan (CSS styling)
2. **Look at your plain HTML page** and imagine what it could look like with styling — colors, fonts, layouts, spacing
3. **Bookmark these resources** (you'll need them next week):
   - Search "CSS Tricks Complete Guide to Flexbox" — bookmark it
   - Search "CSS Tricks Complete Guide to Grid" — bookmark it
   - Search "Google Fonts" — browse some fonts you like

---

## 📊 Week 1 Summary Checklist

| Day | Focus | Completed? |
|-----|-------|:----------:|
| Day 1 | Internet fundamentals + tool setup | ☐ |
| Day 2 | Headings, paragraphs, images, links | ☐ |
| Day 3 | Lists, tables, semantic HTML | ☐ |
| Day 4 | Navigation, anchor links, forms | ☐ |
| Day 5 | Polish, stretch challenges, validation | ☐ |
| Day 6 | Exploration and personal enhancements | ☐ |
| Day 7 | Final review, reflection, plan ahead | ☐ |

### ✅ Project Requirements Checklist
- ☐ Proper `<!DOCTYPE html>` and document structure
- ☐ Heading with your name
- ☐ Paragraph about yourself
- ☐ An image
- ☐ Unordered list of 5 hobbies
- ☐ Ordered list of education/experience
- ☐ Table with weekly schedule
- ☐ Navigation with anchor `#id` links
- ☐ Contact form (name, email, message)
- ☐ Semantic HTML tags (`<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`)
- ☐ **Stretch:** `<details>`/`<summary>` FAQ section
- ☐ **Stretch:** `<meta>` tags for description and viewport
- ☐ **Stretch:** HTML validated at validator.w3.org

---

> 💪 **Remember:** Your page will look plain and unstyled — that is 100% expected. You built a **structurally sound, semantic, accessible** HTML document. That's the foundation everything else is built on. Next week, CSS will transform it into something beautiful.
