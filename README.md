# 🚀 Full Stack AI Engineer — Interview Preparation Guide

> A comprehensive collection of interview questions for Full Stack developers and AI Engineers.
> Covering everything from HTML basics to advanced system design and AI/ML concepts.
> **Level:** 0–5 Years of Experience

---

## 📚 Table of Contents

- [HTML Interview Questions](#-html-interview-questions)
- [CSS Interview Questions](#-css-interview-questions) *(Coming Soon)*
- [JavaScript Interview Questions](#-javascript-interview-questions) *(Coming Soon)*
- [React Interview Questions](#-react-interview-questions) *(Coming Soon)*
- [Node.js Interview Questions](#-nodejs-interview-questions) *(Coming Soon)*
- [Database Interview Questions](#-database-interview-questions) *(Coming Soon)*
- [System Design Questions](#-system-design-questions) *(Coming Soon)*
- [AI/ML Interview Questions](#-aiml-interview-questions) *(Coming Soon)*

---

## 🌐 HTML Interview Questions

> **Level:** Fresher to 5 Years Experience
> **Topics Covered:** Basics, Semantic HTML, Forms, Accessibility, HTML5 APIs, Performance

---

### 📘 Section 1: HTML Basics (Fresher / 0–1 Year)

---

**Q1. What is HTML? What does HTML stand for?**

**Answer:**
HTML stands for **HyperText Markup Language**. It is the standard language used to create and structure content on the web. HTML uses a system of **elements** represented by **tags** to structure text, images, links, and other content.

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My First Page</title>
  </head>
  <body>
    <h1>Hello, World!</h1>
  </body>
</html>
```

---

**Q2. What is the difference between HTML elements and HTML tags?**

**Answer:**
- **Tag:** A tag is the markup notation, e.g., `<p>` (opening tag) and `</p>` (closing tag).
- **Element:** An element includes the opening tag, content, and closing tag together.

```html
<!-- Tag: <p> and </p> -->
<!-- Element: <p>Hello</p> -->
<p>Hello</p>
```

---

**Q3. What is `<!DOCTYPE html>` and why is it important?**

**Answer:**
`<!DOCTYPE html>` is a **document type declaration** that tells the browser which version of HTML the page is written in. For HTML5, it is simply `<!DOCTYPE html>`. Without it, browsers may render the page in **quirks mode**, causing inconsistent behavior.

---

**Q4. What is the difference between block-level and inline elements? Give examples.**

**Answer:**

| Feature | Block-Level | Inline |
|--------|-------------|--------|
| Starts on | New line | Same line |
| Width | Full width | Content width |
| Examples | `<div>`, `<p>`, `<h1>`, `<ul>`, `<table>` | `<span>`, `<a>`, `<strong>`, `<img>` |

```html
<!-- Block: takes full width, new line -->
<p>This is a paragraph.</p>

<!-- Inline: stays in line with text -->
<p>This is <strong>bold</strong> text.</p>
```

---

**Q5. What is the difference between `<div>` and `<span>`?**

**Answer:**
- `<div>` is a **block-level** container used for grouping large sections of content.
- `<span>` is an **inline** container used for styling small parts of text or elements.

```html
<div style="background: lightblue;">Block container</div>
<p>This is <span style="color: red;">inline</span> text.</p>
```

---

**Q6. What are void/self-closing elements in HTML?**

**Answer:**
Void elements are HTML elements that **do not have a closing tag** and cannot contain child elements.

Examples: `<br>`, `<hr>`, `<img>`, `<input>`, `<link>`, `<meta>`

```html
<img src="photo.jpg" alt="A photo" />
<input type="text" placeholder="Enter name" />
<br />
```

---

**Q7. What is the difference between `id` and `class` attributes?**

**Answer:**

| Feature | `id` | `class` |
|--------|------|---------|
| Uniqueness | Must be **unique** on the page | Can be used on **multiple** elements |
| CSS selector | `#id-name` | `.class-name` |
| JS usage | `getElementById()` | `getElementsByClassName()` |

```html
<h1 id="main-title">Unique Title</h1>
<p class="highlight">First highlighted para</p>
<p class="highlight">Second highlighted para</p>
```

---

**Q8. What is the purpose of the `alt` attribute in images?**

**Answer:**
The `alt` attribute provides **alternative text** for an image if it cannot be displayed. It is also crucial for **accessibility** (screen readers) and **SEO**.

```html
<img src="dog.jpg" alt="A golden retriever sitting in a park" />
```

---

**Q9. What is the difference between absolute and relative URLs?**

**Answer:**
- **Absolute URL:** Full URL including protocol and domain. `https://www.example.com/page.html`
- **Relative URL:** Path relative to the current document. `../images/photo.jpg`

```html
<!-- Absolute -->
<a href="https://google.com">Google</a>

<!-- Relative -->
<a href="./about.html">About Us</a>
```

---

**Q10. What are HTML attributes? Give examples.**

**Answer:**
Attributes provide **additional information** about HTML elements. They are placed in the opening tag.

```html
<a href="https://example.com" target="_blank" rel="noopener">Click here</a>
<!--   ^^^^ attribute         ^^^^^^ attribute  ^^^ attribute          -->
```

---

### 📗 Section 2: Semantic HTML (1–2 Years)

---

**Q11. What is Semantic HTML? Why is it important?**

**Answer:**
Semantic HTML uses elements that have **meaningful names** that describe their purpose and content, rather than just defining how they look.

**Benefits:**
- ✅ Better **SEO** (search engines understand content structure)
- ✅ Better **accessibility** (screen readers navigate correctly)
- ✅ Better **code readability** and maintainability

```html
<!-- ❌ Non-semantic -->
<div class="header">
  <div class="nav">...</div>
</div>

<!-- ✅ Semantic -->
<header>
  <nav>...</nav>
</header>
```

---

**Q12. What are the key semantic HTML5 elements? Explain each.**

**Answer:**

| Element | Purpose |
|---------|---------|
| `<header>` | Introductory content or navigation links for a section/page |
| `<nav>` | Navigation links |
| `<main>` | Dominant content of the `<body>` |
| `<article>` | Self-contained, independently distributable content |
| `<section>` | A thematic grouping of content |
| `<aside>` | Content indirectly related to main content (sidebar) |
| `<footer>` | Footer of a section or page |
| `<figure>` | Self-contained content like images with captions |
| `<figcaption>` | Caption for a `<figure>` element |
| `<time>` | A specific time or date |
| `<mark>` | Highlighted/marked text |

```html
<body>
  <header>
    <nav>...</nav>
  </header>
  <main>
    <article>
      <section>
        <h2>Section Title</h2>
        <p>Content here...</p>
      </section>
    </article>
    <aside>Related links</aside>
  </main>
  <footer>© 2025 My Site</footer>
</body>
```

---

**Q13. What is the difference between `<article>` and `<section>`?**

**Answer:**
- `<article>` is for **self-contained** content that can stand alone (blog post, news article, forum post).
- `<section>` is for **thematically grouped** content that is part of a larger whole.

> **Rule of thumb:** If you can share the content independently (RSS feed, repost), use `<article>`. Otherwise, use `<section>`.

---

**Q14. What is the difference between `<strong>` and `<b>`, and `<em>` and `<i>`?**

**Answer:**

| Tags | Visual Effect | Semantic Meaning |
|------|---------------|-----------------|
| `<strong>` | **Bold** | Important, strong importance |
| `<b>` | **Bold** | Stylistically bold, no semantic meaning |
| `<em>` | *Italic* | Emphasized text (stress emphasis) |
| `<i>` | *Italic* | Italic text (technical term, foreign word) |

---

**Q15. What is the `<meta>` tag? What are common meta tags?**

**Answer:**
`<meta>` tags provide **metadata** about the HTML document — information not displayed on the page but used by browsers, search engines, and social media.

```html
<head>
  <!-- Character encoding -->
  <meta charset="UTF-8" />

  <!-- Responsive viewport -->
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />

  <!-- SEO Description -->
  <meta name="description" content="Full stack interview prep guide" />

  <!-- Keywords (less used now) -->
  <meta name="keywords" content="HTML, CSS, JavaScript" />

  <!-- Author -->
  <meta name="author" content="Your Name" />

  <!-- Open Graph (Social sharing) -->
  <meta property="og:title" content="Page Title" />
  <meta property="og:image" content="https://example.com/image.jpg" />
</head>
```

---

### 📙 Section 3: HTML Forms (1–3 Years)

---

**Q16. Explain the key attributes of the HTML `<form>` element.**

**Answer:**

```html
<form
  action="/submit"       <!-- URL where form data is sent -->
  method="POST"          <!-- HTTP method: GET or POST -->
  enctype="multipart/form-data"  <!-- for file uploads -->
  novalidate             <!-- disables native browser validation -->
>
```

| Attribute | Description |
|-----------|-------------|
| `action` | URL to send form data to |
| `method` | `GET` (appends to URL) or `POST` (sends in body) |
| `enctype` | Encoding type; `multipart/form-data` needed for file uploads |
| `novalidate` | Disables browser's built-in validation |

---

**Q17. What is the difference between GET and POST methods in forms?**

**Answer:**

| Feature | GET | POST |
|---------|-----|------|
| Data location | Appended to URL as query string | Sent in request body |
| Visibility | Visible in browser URL | Not visible |
| Security | Less secure | More secure |
| Data size | Limited (~2048 chars) | No practical limit |
| Use case | Search, filtering | Login, file upload, sensitive data |

---

**Q18. What are all the input types available in HTML5?**

**Answer:**
```html
<input type="text" />           <!-- Text field -->
<input type="password" />       <!-- Password (masked) -->
<input type="email" />          <!-- Email validation built-in -->
<input type="number" />         <!-- Numeric input -->
<input type="tel" />            <!-- Telephone number -->
<input type="url" />            <!-- URL validation -->
<input type="date" />           <!-- Date picker -->
<input type="time" />           <!-- Time picker -->
<input type="datetime-local" /> <!-- Date and time -->
<input type="month" />          <!-- Month picker -->
<input type="week" />           <!-- Week picker -->
<input type="range" />          <!-- Slider -->
<input type="color" />          <!-- Color picker -->
<input type="checkbox" />       <!-- Checkbox -->
<input type="radio" />          <!-- Radio button -->
<input type="file" />           <!-- File upload -->
<input type="search" />         <!-- Search field -->
<input type="submit" />         <!-- Submit button -->
<input type="reset" />          <!-- Reset button -->
<input type="button" />         <!-- Generic button -->
<input type="hidden" />         <!-- Hidden field -->
<input type="image" />          <!-- Image as submit button -->
```

---

**Q19. What is the purpose of `<label>` in forms? How do you associate it with an input?**

**Answer:**
`<label>` improves **accessibility** and **usability** — clicking the label focuses the associated input.

```html
<!-- Method 1: Using 'for' and 'id' -->
<label for="username">Username:</label>
<input type="text" id="username" name="username" />

<!-- Method 2: Wrapping the input -->
<label>
  Email:
  <input type="email" name="email" />
</label>
```

---

**Q20. What are HTML5 form validation attributes?**

**Answer:**
```html
<input type="text"
  required                   <!-- Field must be filled -->
  minlength="3"              <!-- Minimum character length -->
  maxlength="50"             <!-- Maximum character length -->
  min="1"                    <!-- Minimum value (numbers/dates) -->
  max="100"                  <!-- Maximum value -->
  pattern="[A-Za-z]{3,}"    <!-- Regex pattern -->
  placeholder="Enter name"   <!-- Hint text -->
  autocomplete="off"         <!-- Disable autocomplete -->
  readonly                   <!-- Cannot edit -->
  disabled                   <!-- Cannot interact at all -->
/>
```

---

**Q21. What is the difference between `disabled` and `readonly` attributes?**

**Answer:**

| Feature | `disabled` | `readonly` |
|---------|-----------|----------|
| User can type | ❌ No | ❌ No |
| Focusable | ❌ No | ✅ Yes |
| Submitted with form | ❌ No | ✅ Yes |
| CSS styling | Grayed out | Normal |

---

### 📕 Section 4: HTML5 APIs & Advanced Concepts (2–4 Years)

---

**Q22. What are HTML5 Web Storage APIs? Difference between `localStorage` and `sessionStorage`?**

**Answer:**

| Feature | `localStorage` | `sessionStorage` |
|---------|---------------|-----------------|
| Persistence | Until manually cleared | Until tab is closed |
| Scope | Same origin, all tabs | Same tab only |
| Storage limit | ~5–10MB | ~5MB |

```javascript
// localStorage
localStorage.setItem('user', 'John');
localStorage.getItem('user');  // "John"
localStorage.removeItem('user');
localStorage.clear();

// sessionStorage
sessionStorage.setItem('token', 'abc123');
sessionStorage.getItem('token');
```

---

**Q23. What is the HTML5 Canvas element? What is it used for?**

**Answer:**
`<canvas>` provides a **bitmap drawing surface** controlled by JavaScript. Used for:
- 2D/3D graphics and animations
- Games
- Data visualizations
- Image manipulation

```html
<canvas id="myCanvas" width="400" height="200"></canvas>

<script>
  const canvas = document.getElementById('myCanvas');
  const ctx = canvas.getContext('2d');
  ctx.fillStyle = 'blue';
  ctx.fillRect(10, 10, 150, 100);
</script>
```

---

**Q24. What is the Geolocation API in HTML5?**

**Answer:**
The Geolocation API allows websites to access the user's **geographical location** (with permission).

```javascript
if (navigator.geolocation) {
  navigator.geolocation.getCurrentPosition(
    (position) => {
      console.log('Lat:', position.coords.latitude);
      console.log('Lng:', position.coords.longitude);
    },
    (error) => {
      console.error('Error:', error.message);
    }
  );
}
```

---

**Q25. What are data attributes (`data-*`) in HTML5?**

**Answer:**
Custom `data-*` attributes allow you to store **extra information** on HTML elements without using non-standard attributes.

```html
<button data-user-id="42" data-role="admin" onclick="handleClick(this)">
  Click Me
</button>

<script>
  function handleClick(el) {
    console.log(el.dataset.userId);  // "42"
    console.log(el.dataset.role);    // "admin"
  }
</script>
```

---

**Q26. What is the `<template>` element in HTML5?**

**Answer:**
`<template>` holds **client-side content** that won't be rendered when the page loads but can be **instantiated via JavaScript**. Useful for reusable HTML fragments.

```html
<template id="card-template">
  <div class="card">
    <h3 class="card-title"></h3>
    <p class="card-desc"></p>
  </div>
</template>

<script>
  const template = document.getElementById('card-template');
  const clone = template.content.cloneNode(true);
  clone.querySelector('.card-title').textContent = 'Hello!';
  document.body.appendChild(clone);
</script>
```

---

**Q27. What is the difference between `<script>`, `<script async>`, and `<script defer>`?**

**Answer:**

| | `<script>` | `<script async>` | `<script defer>` |
|--|-----------|-----------------|-----------------|
| Parsing paused | ✅ Yes | ✅ While executing | ❌ No |
| Execution timing | Immediately | As soon as downloaded | After HTML parsed |
| Order guaranteed | ✅ Yes | ❌ No | ✅ Yes |
| Use case | Critical scripts | Analytics, ads | General scripts |

```html
<!-- Blocks parsing -->
<script src="app.js"></script>

<!-- Downloads in parallel, executes ASAP -->
<script async src="analytics.js"></script>

<!-- Downloads in parallel, executes after DOM ready -->
<script defer src="main.js"></script>
```

---

**Q28. What is the Shadow DOM? How is it related to Web Components?**

**Answer:**
The **Shadow DOM** is a browser API that attaches a hidden, isolated DOM tree to an element — styles and scripts inside do not affect the main document.

**Web Components** are made of:
1. **Custom Elements** – define new HTML elements
2. **Shadow DOM** – encapsulated styles/markup
3. **HTML Templates** – reusable markup

```javascript
class MyCard extends HTMLElement {
  constructor() {
    super();
    const shadow = this.attachShadow({ mode: 'open' });
    shadow.innerHTML = `
      <style>p { color: red; }</style>
      <p>Shadow DOM content</p>
    `;
  }
}
customElements.define('my-card', MyCard);
```
```html
<my-card></my-card>
```

---

### 📓 Section 5: Accessibility & Best Practices (3–5 Years)

---

**Q29. What is ARIA? Why and how is it used?**

**Answer:**
**ARIA (Accessible Rich Internet Applications)** is a set of attributes that add **accessibility semantics** to HTML, helping screen readers understand dynamic content.

```html
<!-- Role -->
<div role="alert">Form submitted successfully!</div>

<!-- State -->
<button aria-pressed="false" id="toggle">Toggle Dark Mode</button>

<!-- Label (when no visible label exists) -->
<button aria-label="Close dialog">✕</button>

<!-- Live region -->
<div aria-live="polite" id="status-message"></div>

<!-- Describe relationship -->
<input type="text" aria-describedby="hint" />
<span id="hint">Must be 6–12 characters</span>
```

> **Rule:** Use native semantic HTML first. Add ARIA only when semantics cannot be achieved with HTML alone.

---

**Q30. What are the WCAG accessibility guidelines? Name a few key principles.**

**Answer:**
**WCAG (Web Content Accessibility Guidelines)** are standards for making web content accessible. The 4 core principles are **POUR**:

| Principle | Meaning |
|-----------|---------|
| **P**erceivable | Information must be presentable in ways users can perceive (alt text, captions) |
| **O**perable | Interface must be navigable (keyboard accessible, no seizure-inducing content) |
| **U**nderstandable | Content must be readable and predictable (clear language, error handling) |
| **R**obust | Content must be interpreted by assistive technologies |

---

**Q31. How do you make a website keyboard accessible?**

**Answer:**
- Use **semantic HTML** (buttons, links, form elements are natively focusable)
- Ensure logical **tab order** (`tabindex`)
- Provide **visible focus indicators** (`:focus` styles)
- Handle **keyboard events** (`keydown`, `keyup`)
- Avoid `outline: none` without an alternative

```html
<!-- Avoid: div acting as button is not keyboard accessible -->
<div onclick="submit()">Submit</div>

<!-- Correct: use real button -->
<button onclick="submit()">Submit</button>
```

---

**Q32. What is the difference between `<link>` and `<a>` tags?**

**Answer:**

| Feature | `<link>` | `<a>` |
|---------|---------|-------|
| Location | Inside `<head>` | Inside `<body>` |
| Purpose | Link external resources (CSS, favicons) | Hyperlinks for navigation |
| User visible | ❌ No | ✅ Yes |

```html
<!-- <link> for external resources -->
<link rel="stylesheet" href="styles.css" />
<link rel="icon" href="favicon.ico" />

<!-- <a> for navigation -->
<a href="https://example.com" target="_blank">Visit</a>
```

---

**Q33. What is the `viewport` meta tag? Why is it important for responsive design?**

**Answer:**
The viewport meta tag controls how the browser **scales the page** on mobile devices.

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

- `width=device-width` — sets page width to match screen width
- `initial-scale=1.0` — sets initial zoom level to 100%

Without it, mobile browsers zoom out to fit the desktop layout, making text tiny.

---

**Q34. What is the difference between `<head>` and `<body>` in HTML?**

**Answer:**

| Feature | `<head>` | `<body>` |
|---------|---------|---------|
| Visibility | Not rendered on page | Visible to users |
| Contains | Metadata, CSS links, title, scripts | Actual page content |
| Purpose | Document configuration | Page presentation |

---

**Q35. What is an iframe? What are its security concerns?**

**Answer:**
`<iframe>` embeds another HTML page **within the current page**.

```html
<iframe
  src="https://www.youtube.com/embed/dQw4w9WgXcQ"
  width="560"
  height="315"
  title="YouTube video"
  allowfullscreen
  loading="lazy"
></iframe>
```

**Security Concerns:**
- **Clickjacking** — attacker embeds your site in an iframe to trick users
- **XSS attacks** — malicious iframes injecting scripts

**Mitigations:**
```html
<!-- Sandbox restricts iframe capabilities -->
<iframe src="content.html" sandbox="allow-scripts allow-same-origin"></iframe>
```
```http
<!-- Prevent your site from being embedded -->
X-Frame-Options: DENY
Content-Security-Policy: frame-ancestors 'none';
```

---

**Q36. What is the difference between `<picture>` and `<img>` elements?**

**Answer:**
`<picture>` provides **art direction** — serving different images based on viewport, resolution, or format support.

```html
<!-- Simple image -->
<img src="photo.jpg" alt="A photo" />

<!-- Responsive / art direction image -->
<picture>
  <!-- Modern WebP format -->
  <source srcset="photo.webp" type="image/webp" />
  <!-- Smaller image for mobile -->
  <source srcset="photo-mobile.jpg" media="(max-width: 600px)" />
  <!-- Fallback -->
  <img src="photo.jpg" alt="A photo" />
</picture>
```

---

**Q37. What is lazy loading in HTML? How do you implement it?**

**Answer:**
Lazy loading **defers loading** of off-screen resources until the user scrolls near them — improving initial page load performance.

```html
<!-- Native lazy loading for images -->
<img src="large-image.jpg" alt="Hero" loading="lazy" />

<!-- Lazy loading iframes -->
<iframe src="video.html" loading="lazy"></iframe>
```

Values: `loading="lazy"` | `loading="eager"` (default)

---

**Q38. What is the HTML `<details>` and `<summary>` element?**

**Answer:**
Creates a **native disclosure widget** (accordion) without JavaScript.

```html
<details>
  <summary>What is HTML?</summary>
  <p>
    HTML stands for HyperText Markup Language and is the standard
    language for creating web pages.
  </p>
</details>
```

---

**Q39. Explain the concept of the Critical Rendering Path.**

**Answer:**
The **Critical Rendering Path** is the sequence of steps the browser takes to convert HTML, CSS, and JS into pixels on the screen:

1. **Parse HTML** → Build DOM tree
2. **Parse CSS** → Build CSSOM tree
3. **Combine** → Render tree
4. **Layout** → Calculate positions and sizes
5. **Paint** → Draw pixels to screen

**Optimization Tips:**
- Place CSS in `<head>` (render-blocking but needed early)
- Place `<script>` at bottom or use `defer`/`async`
- Minimize render-blocking resources
- Use `<link rel="preload">` for critical resources

---

**Q40. What are some best practices for writing clean, maintainable HTML?**

**Answer:**

✅ **Do:**
- Use semantic elements (`<header>`, `<nav>`, `<main>`, etc.)
- Always include `alt` text on images
- Use lowercase for tags and attributes
- Quote all attribute values
- Keep HTML structure flat where possible
- Use `id` only for unique elements
- Validate HTML with [W3C Validator](https://validator.w3.org/)

❌ **Avoid:**
- Using `<div>` and `<span>` for everything
- Inline styles (use CSS classes instead)
- Deprecated tags (`<font>`, `<center>`, `<marquee>`)
- Skipping heading levels (h1 → h3, skipping h2)
- Empty `alt` attributes on meaningful images

---

## 🎯 Quick Revision Cheatsheet

| Concept | Key Points |
|---------|-----------|
| **DOCTYPE** | Tells browser HTML version; prevents quirks mode |
| **Semantic HTML** | Meaningful tags → better SEO + accessibility |
| **Block vs Inline** | Block = full width; Inline = content width |
| **id vs class** | id = unique; class = reusable |
| **GET vs POST** | GET = URL params; POST = request body |
| **defer vs async** | defer = ordered, after DOM; async = unordered, ASAP |
| **localStorage** | Persists until cleared; sessionStorage = tab only |
| **ARIA** | Accessibility attributes for dynamic content |
| **lazy loading** | `loading="lazy"` on `<img>` and `<iframe>` |
| **Shadow DOM** | Encapsulated DOM for Web Components |

---

## 📌 Coming Next

| Topic | Status |
|-------|--------|
| 🎨 CSS Interview Questions | 🔜 Coming Soon |
| ⚡ JavaScript Interview Questions | 🔜 Coming Soon |
| ⚛️ React Interview Questions | 🔜 Coming Soon |
| 🟢 Node.js Interview Questions | 🔜 Coming Soon |
| 🗄️ Database (SQL + NoSQL) | 🔜 Coming Soon |
| 🏗️ System Design | 🔜 Coming Soon |
| 🤖 AI/ML for Engineers | 🔜 Coming Soon |

---

## 🤝 Contributing

Feel free to open issues or PRs to add more questions, fix answers, or improve explanations!

---

## ⭐ Star this repo if it helped you!

> Made with ❤️ for developers preparing for Full Stack & AI Engineering interviews.
