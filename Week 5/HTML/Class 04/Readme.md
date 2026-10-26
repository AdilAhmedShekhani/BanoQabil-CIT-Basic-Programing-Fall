# Class 4: HTML Media, Semantic Tags & Introduction to CSS

Welcome to Class 4! In this session, we explore multimedia elements in HTML (`<video>` and `<audio>`), modern **Semantic Tags** for clean web structure, and take our first steps into styling web pages with **CSS**.

---

## 📌 Table of Contents

1. [HTML Media Tags](#1-html-media-tags)
   * Video Tag (`<video>`)
   * Audio Tag (`<audio>`)
2. [Semantic HTML Tags](#2-semantic-html-tags)
   * Why use Semantic Tags?
   * Key Semantic Elements (`header`, `nav`, `main`, `section`, `article`, `footer`)
3. [Introduction to CSS](#3-introduction-to-css)
   * What is CSS?
   * 3 Ways to Apply CSS (Inline, Internal, External)
   * Targeting Headings (`<h1>`-`<h6>`) and Paragraphs (`<p>`)

---

## 1. HTML Media Tags

### A. The `<video>` Tag
Used to embed video clips directly into your web pages.

**Common Attributes:**
* `src`: The path/URL of the video file.
* `controls`: Displays video controls (play, pause, volume).
* `width` / `height`: Sets dimensions.
* `autoplay`: Plays the video automatically (requires `muted` in most browsers).
* `loop`: Repeats the video after it finishes.

```html
<!-- Basic Video Player -->
<video src="media/sample.mp4" controls width="600">
  Your browser does not support the video tag.
</video>
```

---

### B. The `<audio>` Tag
Used to embed sound content or audio streams.

**Common Attributes:**
* `src`: Path to the audio file.
* `controls`: Adds play, pause, and volume controls.
* `autoplay`: Plays audio automatically on page load.
* `loop`: Loops the audio endlessly.

```html
<!-- Basic Audio Player -->
<audio src="media/podcast.mp3" controls>
  Your browser does not support the audio tag.
</audio>
```

---

## 2. Semantic HTML Tags

Semantic HTML tags clearly describe their meaning to both the browser and the developer. Instead of using `<div>` for everything, semantic tags give structure and improve **SEO** and **Accessibility**.

### Commonly Used Semantic Tags:

* `<header>`: Contains introductory content, logos, or main navigation.
* `<nav>`: Contains navigation links (`<a>`).
* `<main>`: Holds the primary, unique content of the web page.
* `<section>`: Groups related content together into logical sections.
* `<article>`: Represents independent, self-contained content (blog posts, news items).
* `<aside>`: Contains secondary content like sidebars or ads.
* `<footer>`: Appears at the bottom of the page (copyright, contact links).

### Example Structure:

```html
<header>
  <h1>My Awesome Website</h1>
  <nav>
    <a href="#">Home</a>
    <a href="#">About</a>
  </nav>
</header>

<main>
  <section>
    <h2>Latest News</h2>
    <p>Welcome to our new website layout built with semantic tags!</p>
  </section>
</main>

<footer>
  <p>&copy; 2026 Web Dev Course. All rights reserved.</p>
</footer>
```

---

## 3. Introduction to CSS

### What is CSS?
**CSS (Cascading Style Sheets)** is used to style and layout web pages—for example, altering fonts, colors, spacing, and positioning.

---

### 3 Ways to Include CSS:

#### 1. Inline CSS
Applied directly inside an HTML tag using the `style` attribute. Useful for quick testing, but not recommended for large projects.

```html
<h1 style="color: blue; text-align: center;">Welcome to Inline CSS</h1>
<p style="color: gray; font-size: 18px;">This paragraph is styled inline.</p>
```

---

#### 2. Internal CSS
Written inside a `<style>` tag within the `<head>` section of an HTML document. Good for single-page styling.

```html
<!DOCTYPE html>
<html>
<head>
  <style>
    /* Target all h1 headings */
    h1 {
      color: darkgreen;
      text-align: center;
    }

    /* Target all paragraphs */
    p {
      color: darkslategray;
      font-size: 16px;
      line-height: 1.5;
    }
  </style>
</head>
<body>
  <h1>Internal CSS Example</h1>
  <p>This paragraph is styled using Internal CSS inside the head section.</p>
</body>
</html>
```

---

#### 3. External CSS
CSS is written in a separate `.css` file (e.g., `style.css`) and linked to the HTML document via the `<link>` tag. **Best practice for web development.**

**File Structure:**
```text
my-project/
├── index.html
└── style.css
```

**Step A: Link the file in `index.html`**
```html
<head>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <h1>External CSS Header</h1>
  <p>This paragraph gets its styling from style.css!</p>
</body>
```

**Step B: Write rules in `style.css`**
```css
/* Targeting Heading Tags */
h1 {
  color: crimson;
  font-family: Arial, sans-serif;
}

/* Targeting Paragraph Tags */
p {
  color: #333333;
  font-size: 18px;
  background-color: #f4f4f4;
  padding: 10px;
}
```

---

## 🎯 Class Assignment / Homework

1. Create a webpage with a `<header>`, `<main>`, and `<footer>` using **Semantic Tags**.
2. Embed an `<audio>` player and a `<video>` player in the `<main>` section with `controls` enabled.
3. Create an external file `style.css` and link it to your HTML file.
4. Target all `<h1>` elements to change their color and center align them.
5. Target all `<p>` elements to change their font size, text color, and background color.
