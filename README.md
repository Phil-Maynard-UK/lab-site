# Lab Site – Static Consultancy Website Starter

This repository contains a simple, static website template designed for small consultancies and solo practitioners.

It is intentionally:
- lightweight
- low-cost
- easy to host
- easy to customise
- free of build tools or complex dependencies

The site is built with plain HTML, CSS, and Bootstrap, and is suitable for hosting on platforms like Cloudflare Pages or GitHub Pages.

---

## What this site is for

This site is designed to act as:
- an “extended business card”
- a calm landing page explaining what you do
- a place to signpost people to book a call or get in touch

It works well for:
- early-stage consultancies
- independent consultants
- people who don’t want to maintain a CMS
- sites that change occasionally rather than weekly

---

## Site structure
````
/
├── index.html # Main landing page (single-page layout)
├── about.html # About page
├── bookacall.html # Booking page (designed to host an embedded calendar)
├── css/
│ └── styles.css # Main stylesheet (includes branding variables)
├── js/
│ └── scripts.js # Minimal JavaScript (Bootstrap behaviour)
├── assets/
│ ├── img/ # Images used by the template
│ └── favicon.ico
└── README.md
````

There is no build step and no server-side code.

---

## How to customise the site

### 1. Change the text content

Most content lives directly in the HTML files.

Safe things to edit:
- headings (`<h1>`, `<h2>`, `<h3>`)
- paragraphs (`<p>`)
- lists (`<ul>`, `<li>`)
- link URLs and link text

Each major section in `index.html` is clearly marked with comments explaining what it is and what can be changed.

You do **not** need to understand HTML deeply to update text.

---

### 2. Change the brand colours

All brand colours are controlled via CSS variables near the bottom of:

````css/styles.css````


Look for a section like:

```css
:root {
  --brand-primary: #3a5f7d;
  --brand-primary-hover: #2f4e66;
  --brand-secondary: #e8b04d;
  --brand-dark: #1f2a33;
}
````
Changing these values will update:
- buttons
- navigation highlights
- icons and accents
- footer links
- You do not need to search-and-replace colours across the site.

