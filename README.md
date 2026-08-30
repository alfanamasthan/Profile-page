# HTML Basics Guide

A simple guide explaining basic HTML tags, structural layout rules, and how to link pages and images correctly.

---

## 1. Headings  Tags

### Heading Tags (`<h1>` to `<h6>`)
Headings are used to create titles and subtitles on your webpage. They show which info is most important.
* **`<h1>`**: The main title of the page. You should only use **one** `<h1>` tag per page.
* **`<h2>` to `<h6>`**: Subtitles used to break your page into smaller sections.
* *Tip:* Always go in order. Do not skip levels (for example, do not jump from `<h1>` straight to `<h3>`).

###  HTML5 Semantic Tags
Semantic tags are words that tell the browser exactly what kind of content is inside them. They make your code easy to read.

* **`<header>`**: Used for the top section of your website. It usually holds the logo, website name, or navigation menu.
* **`<main>`**: Wraps the most important, unique content of your webpage. You are only allowed **one** `<main>` tag per page.
* **`<footer>`**: Used for the very bottom section of your website. It usually holds copyright notes, links, or contact info.

---

##  2. Links and Image Paths

###  The Anchor Tag (`<a>`)
The anchor tag is used to create clickable links. It uses the `href` attribute to know where to send the user.
```html
<!-- Opens the link in the same browser tab -->
<a href="https://github.com">Go to My GitHub</a>

<!-- target="_blank" opens the link in a completely new tab -->
<a href="https://github.com" target="_blank">Open GitHub in New Tab</a>
```

###  The Image Tag (`<img>`) and File Paths
The `<img>` tag puts pictures onto your website. It needs a `src` attribute (where the image file is saved) and an `alt` attribute (text that describes the image if it fails to load).

#### Absolute Path vs. Relative Path
* **Absolute Path:** The full website address from the internet. It points to a file saved on another website.
* **Relative Path:** A path that points to a file inside your own project folder.

```html
<!-- Absolute Path Example (links to an external website) -->
<img src="https://example.com" alt="Company Logo">

<!-- Relative Path Example (links to a file inside your local folder) -->
<img src="./public/html.png" alt="HTML Logo" width="50" height="50">
```

---

## 3. Creating Lists (`<ul>` and `<ol>`)

Lists help you organize items neatly. Every single item inside a list must be wrapped in a list item (`<li>`) tag.

### Unordered List (`<ul>`)
Creates a bulleted list. Use this when the order of items does not matter.

### Ordered List (`<ol>`)
Creates a numbered list. Use this when the order or steps do matter. It can use extra attributes:

```html
<!-- An ordered list  -->
<ol >
  <li>This item will show up with the number V</li>
  <li>This item will show up with the number VI</li>
</ol>
```

---

## 4. Boxes and Text Styling: `<div>` vs. `<span>`

When there isn't a special tag for your layout, you can use these two tags to group your elements together for CSS styling.

### `<div>` (Block-Level)
* **How it works:** It acts like a big box that takes up the **full width** of the screen.
* **Rule:** It automatically pushes any content that comes after it down to a brand new line.

### `<span>` (Inline-Level)
* **How it works:** It only takes up as much space as the text inside it needs.
* **Rule:** It stays right inside the same line of text without creating a new line. It is perfect for styling a single word.

```html
<!-- A DIV box separating content onto its own line -->
<div>
  <h3>Section Box</h3>
  <p>All of this content stays inside one big layout box.</p>
</div>

<!-- A SPAN tag styling a single word inside a sentence -->
<p>Coding is very <span style="color: blue;">fun</span> to learn!</p>
```
