# Class 3: HTML Links & Tables

Welcome to Class 3 of our Web Development course! In this session, we covered how to connect web pages using **Anchor Tags** and how to display structured data using **HTML Tables**.

---

## 📌 Table of Contents
1. [Anchor Tags (`<a>`)](#1-anchor-tags-a)
   - External Links (Social Networks, external sites)
   - Internal Links (Connecting multiple pages)
2. [HTML Tables (`<table>`)](#2-html-tables-table)
   - Table Elements (`tr`, `th`, `td`, `thead`, `tbody`, `tfoot`)
   - Adding Borders using Attributes

---

## 1. Anchor Tags (`<a>`)

The `<a>` (anchor) tag is used to create hyperlinks, which allow users to navigate from one page to another.

### A. External Links
External links take users to a different website on the internet (e.g., Facebook, LinkedIn, Google).

**Attributes used:**
* `href`: Specifies the URL (destination address) of the page.
* `target="_blank"`: Opens the linked document in a new tab/window.

```html
<!-- Link to Facebook -->
<a href="https://www.facebook.com" target="_blank">Visit Facebook</a>

<!-- Link to LinkedIn -->
<a href="https://www.linkedin.com" target="_blank">Visit LinkedIn</a>
```

---

### B. Internal Links (Multi-page Navigation)
Internal links connect different pages within your own website directory.

#### Project Folder Structure Example:
```text
my-website/
├── index.html
├── about.html
└── contact.html
```

#### Example Usage:

**In `index.html`:**
```html
<nav>
  <a href="index.html">Home</a> | 
  <a href="about.html">About Us</a> | 
  <a href="contact.html">Contact Us</a>
</nav>
```

---

## 2. HTML Tables (`<table>`)

Tables are used to display data in a structured, grid-like format consisting of rows and columns.

### Key Table Tags:
* `<table>`: Wraps the entire table content.
* `<thead>`: Groups the header content of the table.
* `<tbody>`: Groups the main body content of the table.
* `<tfoot>`: Groups the footer content of the table (optional).
* `<tr>` *(Table Row)*: Defines a single row.
* `<th>` *(Table Header)*: Defines a header cell (bold and centered by default).
* `<td>` *(Table Data)*: Defines a standard data cell.

---

### Adding Borders using Attributes
You can add a basic border directly to your table using the `border` attribute inside the `<table>` tag.

> **Note:** Modern websites use CSS for styling, but using the `border` attribute is a great way to visualize tables when learning basic HTML.

---

### Full Table Example:

```html
<table border="1">
  <thead>
    <tr>
      <th>Roll No</th>
      <th>Name</th>
      <th>Course</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>101</td>
      <td>Ali Khan</td>
      <td>Web Development</td>
    </tr>
    <tr>
      <td>102</td>
      <td>Sara Ahmed</td>
      <td>Graphic Design</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td colspan="3">Total Students: 2</td>
    </tr>
  </tfoot>
</table>
```

---

## 🎯 Class Assignment / Homework
1. Create a 3-page website (`index.html`, `about.html`, `contact.html`) linked together using anchor tags.
2. Add links to your social media profiles (LinkedIn, GitHub, Facebook) on the `contact.html` page using `target="_blank"`.
3. Create a timetable or student record table on the `index.html` page using all table elements (`table`, `thead`, `tbody`, `tr`, `th`, `td`) with a `border` attribute.
