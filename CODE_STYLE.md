# Code Style Guide - HTML & CSS Standards

This document outlines the coding standards and best practices used in the Preliminaries of Web repository. Following these guidelines ensures consistency, readability, and maintainability of code.

---

## 🏗️ HTML Coding Standards

### 1. Document Structure

#### Proper HTML5 Template
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Page Title</title>
</head>
<body>
    <!-- Content goes here -->
</body>
</html>
```

**Standards**:
- ✅ Always use `<!DOCTYPE html>` for HTML5
- ✅ Always include `lang` attribute in `<html>` tag
- ✅ Always include `<meta charset="UTF-8">` in `<head>`
- ✅ Always include viewport meta tag for responsive design
- ✅ Put CSS in `<head>` or external file
- ✅ Put JavaScript before closing `</body>` tag

### 2. Indentation and Formatting

#### Indentation Rules
```html
<!-- Use 4 spaces or 1 tab for indentation -->
<div>
    <p>Content here</p>
    <ul>
        <li>Item 1</li>
        <li>Item 2</li>
    </ul>
</div>
```

**Standards**:
- ✅ Use consistent indentation (4 spaces recommended)
- ✅ Each nested level gets one indentation
- ✅ Closing tags should align with opening tags
- ✅ Use one element per line (except inline elements)

#### Proper Formatting
```html
<!-- GOOD: Clear and readable -->
<table>
    <tr>
        <th>Header 1</th>
        <th>Header 2</th>
    </tr>
    <tr>
        <td>Data 1</td>
        <td>Data 2</td>
    </tr>
</table>

<!-- BAD: Hard to read -->
<table><tr><th>Header 1</th><th>Header 2</th></tr><tr><td>Data 1</td><td>Data 2</td></tr></table>
```

### 3. Attribute Formatting

#### Single vs. Double Quotes
```html
<!-- GOOD: Use double quotes -->
<img src="image.jpg" alt="Description">
<a href="page.html" title="Link title">

<!-- AVOID: Single quotes (unless necessary) -->
<img src='image.jpg' alt='Description'>
```

**Standards**:
- ✅ Use double quotes for attributes
- ✅ Always include quotes around attribute values
- ✅ Ordered attributes: id, class, data-*, other attributes

#### Attribute Order
```html
<!-- GOOD: Logical attribute order -->
<input id="email" class="form-field" type="email" name="email" required>
<div id="header" class="container" data-type="header">

<!-- Order: id, class, type/name, other specific, generic -->
```

### 4. Semantic HTML

#### Use Meaningful Elements
```html
<!-- GOOD: Semantic elements -->
<header>
    <nav>Navigation</nav>
</header>
<main>
    <article>Content</article>
    <aside>Sidebar</aside>
</main>
<footer>Footer</footer>

<!-- BAD: Generic divs -->
<div id="header">
    <div id="nav">Navigation</div>
</div>
<div id="main">
    <div id="article">Content</div>
    <div id="sidebar">Sidebar</div>
</div>
```

**Semantic Elements**:
- `<header>` - Page header
- `<nav>` - Navigation section
- `<main>` - Main content
- `<article>` - Self-contained article
- `<section>` - Thematic grouping
- `<aside>` - Sidebar content
- `<footer>` - Page footer

### 5. Specific HTML Elements

#### Images
```html
<!-- GOOD: Always include alt text -->
<img src="profile.jpg" alt="User profile picture" width="200" height="200">

<!-- BAD: Missing alt text -->
<img src="profile.jpg">
```

**Standards**:
- ✅ Always include descriptive `alt` text
- ✅ Include `width` and `height` to prevent layout shift
- ✅ Use appropriate image formats
- ✅ Optimize images for web

#### Links
```html
<!-- GOOD: Descriptive link text -->
<a href="/about">Learn more about us</a>
<a href="contact.html">Contact page</a>

<!-- BAD: Generic link text -->
<a href="/about">Click here</a>
<a href="contact.html">Link</a>
```

**Standards**:
- ✅ Use descriptive link text
- ✅ Avoid "click here" or generic text
- ✅ Use absolute paths for external links
- ✅ Use relative paths for internal links

#### Forms
```html
<!-- GOOD: Proper form structure -->
<form id="contact" method="POST" action="/submit">
    <label for="name">Name:</label>
    <input id="name" type="text" name="name" required>
    
    <label for="email">Email:</label>
    <input id="email" type="email" name="email" required>
    
    <button type="submit">Send</button>
</form>

<!-- BAD: Missing labels, unclear structure -->
<form>
    Name: <input type="text" name="name">
    Email: <input type="email">
    <button>Send</button>
</form>
```

**Standards**:
- ✅ Always use `<label>` elements with `for` attribute
- ✅ Use appropriate `type` attributes for inputs
- ✅ Use `required` attribute for mandatory fields
- ✅ Use `<fieldset>` for grouped form elements

#### Lists
```html
<!-- GOOD: Proper list structure -->
<ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
</ul>

<!-- Definition list -->
<dl>
    <dt>Term</dt>
    <dd>Definition</dd>
</dl>

<!-- BAD: Incorrect list usage -->
<p>• Item 1<br>• Item 2<br>• Item 3</p>
```

### 6. Comments

#### Comment Style
```html
<!-- Good: Brief, meaningful comment -->
<!-- Main navigation menu -->
<nav>...</nav>

<!-- Good: Explains complex sections -->
<!-- 
    Product pricing table with:
    - Column headers for price tiers
    - Row headers for features
    - Highlighted best value option
-->
<table>...</table>

<!-- Avoid: Obvious comments -->
<!-- Paragraph with text -->
<p>Text</p>

<!-- Avoid: Commented code (use version control instead) -->
<!-- <p>This was the old version</p> -->
```

---

## 🎨 CSS Coding Standards

### 1. CSS Structure

#### Internal CSS Format
```html
<style>
    /* Grouped by functionality */
    
    /* Layout */
    body {
        margin: 0;
        padding: 10px;
    }
    
    /* Typography */
    h1 {
        font-size: 2em;
        font-weight: bold;
    }
    
    /* Components */
    .button {
        padding: 10px 20px;
        background-color: #007bff;
    }
</style>
```

**Standards**:
- ✅ Group related rules together
- ✅ Use comments to separate sections
- ✅ Maintain consistent formatting
- ✅ One rule per line inside declaration

### 2. Selectors

#### Selector Priority
```css
/* GOOD: Specific selectors */
#header { }          /* ID - Use sparingly */
.nav-item { }        /* Class - Preferred */
nav { }              /* Element - Basic */

/* AVOID: Overly specific */
body div#header nav.nav-item { }
```

**Standards**:
- ✅ Use classes for styling (preferred)
- ✅ Use IDs sparingly, mainly for JavaScript
- ✅ Use element selectors for basic tags
- ✅ Avoid deeply nested selectors

#### Naming Conventions
```css
/* GOOD: Descriptive, lowercase, hyphens */
.primary-button { }
.user-profile-card { }
.form-field-error { }

/* AVOID: Unclear names */
.btn1 { }
.p { }
.item_container { }
```

### 3. CSS Properties

#### Property Organization
```css
/* Organize properties logically */
.component {
    /* Display & Layout */
    display: block;
    position: relative;
    float: none;
    
    /* Sizing */
    width: 100%;
    height: auto;
    
    /* Spacing */
    margin: 10px;
    padding: 15px;
    
    /* Typography */
    font-family: Arial, sans-serif;
    font-size: 14px;
    color: #333;
    
    /* Visual */
    background-color: #fff;
    border: 1px solid #ccc;
    border-radius: 4px;
    
    /* Effects */
    box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    transition: all 0.3s ease;
}
```

**Standard Order**:
1. Display & Layout (`display`, `position`, `float`)
2. Sizing (`width`, `height`, `max-width`)
3. Spacing (`margin`, `padding`)
4. Typography (`font-*`, `color`, `line-height`)
5. Visual (`background`, `border`, `border-radius`)
6. Effects (`box-shadow`, `transition`, `transform`)

### 4. Colors

#### Color Format
```css
/* GOOD: Consistent format */
body {
    background-color: #ffffff;      /* Hex - preferred */
    color: #333333;
}

header {
    background-color: rgb(0, 123, 255);  /* RGB - when needed */
}

footer {
    background-color: rgba(0, 0, 0, 0.9);  /* RGBA - with transparency */
}

/* AVOID: Inconsistent formats in same file */
body {
    background-color: #fff;         /* Short hex */
    color: black;                   /* Named color */
}
```

**Standards**:
- ✅ Use hex colors (e.g., `#333333`)
- ✅ Use `rgb()` and `rgba()` for complex colors
- ✅ Use CSS variables for repeated colors (advanced)
- ✅ Avoid named colors (use hex instead)
- ✅ Be consistent within the same file

### 5. Units and Sizing

#### Unit Usage
```css
/* GOOD: Appropriate units */
body {
    font-size: 16px;           /* Fixed base size */
}

h1 {
    font-size: 2em;            /* Relative to parent */
}

.container {
    width: 100%;               /* Responsive */
    max-width: 1200px;         /* Constraint */
    margin: 0 auto;            /* Center */
}

.btn {
    padding: 10px 20px;        /* Explicit spacing */
}

/* AVOID: Inconsistent units */
body {
    font-size: 16pt;           /* Avoid pt for web */
}

.container {
    width: 960px;              /* Not responsive */
}
```

**Standards**:
- ✅ Use `px` for fixed sizes
- ✅ Use `%` for responsive sizing
- ✅ Use `em` or `rem` for typography
- ✅ Use `auto` for automatic sizing
- ✅ Avoid `pt` for web fonts

### 6. Spacing and Alignment

#### Margin and Padding
```css
/* GOOD: Shorthand when consistent */
.box {
    margin: 10px;              /* All sides */
    padding: 20px 10px;        /* Vertical Horizontal */
}

/* GOOD: Explicit when different */
.box {
    margin-top: 10px;
    margin-bottom: 20px;
    padding-left: 15px;
}

/* AVOID: Redundant */
.box {
    margin-top: 10px;
    margin-right: 10px;
    margin-bottom: 10px;
    margin-left: 10px;
    /* Use: margin: 10px; instead */
}
```

### 7. Specificity and Cascading

#### Avoid High Specificity
```css
/* GOOD: Low specificity */
.button {
    background-color: blue;
}

.button-primary {
    background-color: darkblue;
}

/* AVOID: High specificity */
body > div > .container > button.button-primary {
    background-color: darkblue;
}
```

**Standards**:
- ✅ Keep specificity low
- ✅ Rely on cascading
- ✅ Use classes for styling
- ✅ Avoid `!important`

---

## 🔍 Validation and Best Practices

### HTML Validation
```bash
# Validate HTML structure
# Use online validators:
# - https://validator.w3.org/
# - https://html5.validator.nu/
```

**Check for**:
- ✅ Valid HTML5 structure
- ✅ Proper nesting of elements
- ✅ All required attributes
- ✅ No deprecated elements

### CSS Validation
```bash
# Validate CSS syntax
# Use online validators:
# - https://jigsaw.w3.org/css-validator/
# - https://codebeautify.org/css-validator
```

**Check for**:
- ✅ Valid CSS syntax
- ✅ Consistent formatting
- ✅ Browser compatibility
- ✅ Performance issues

### Accessibility Standards
```html
<!-- GOOD: Accessible markup -->
<img src="photo.jpg" alt="Descriptive alt text">
<button>Action</button>
<label for="input">Label:</label>
<input id="input" type="text">

<!-- BAD: Accessibility issues -->
<img src="photo.jpg" alt="">
<div onclick="action()">Action</div>
<div>Label:</div>
<input type="text">
```

**Accessibility Checklist**:
- ✅ Proper heading hierarchy
- ✅ Descriptive alt text
- ✅ Semantic HTML elements
- ✅ Keyboard navigation
- ✅ Color contrast
- ✅ Labels for form inputs

---

## 📋 Code Review Checklist

Before submitting code, ensure:

### HTML
- [ ] Valid HTML5 structure
- [ ] Proper indentation
- [ ] Semantic elements used correctly
- [ ] All images have alt text
- [ ] All links are descriptive
- [ ] Forms have proper labels
- [ ] Comments are meaningful
- [ ] No inline styles (use CSS)

### CSS
- [ ] Valid CSS syntax
- [ ] Consistent color format
- [ ] Proper selector naming
- [ ] Reasonable specificity
- [ ] Consistent property order
- [ ] Grouped by functionality
- [ ] Comments for complex rules
- [ ] Cross-browser compatible

### Overall
- [ ] Code is readable and maintainable
- [ ] Consistent with project style
- [ ] No commented-out code
- [ ] No debug code left in
- [ ] Optimized for performance
- [ ] Tested in multiple browsers

---

## 🚀 Quick Reference

### Common HTML5 Template
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Page Title</title>
    <style>
        /* CSS here */
    </style>
</head>
<body>
    <header>
        <h1>Page Title</h1>
    </header>
    <main>
        <!-- Content -->
    </main>
    <footer>
        <!-- Footer content -->
    </footer>
</body>
</html>
```

### CSS Starter Template
```css
/* Reset and Base Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Arial', sans-serif;
    font-size: 16px;
    line-height: 1.6;
    color: #333;
}

/* Layout */
.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* Typography */
h1, h2, h3 {
    font-weight: bold;
    line-height: 1.2;
}

h1 { font-size: 2em; }
h2 { font-size: 1.5em; }
h3 { font-size: 1.2em; }

/* Components */
.button {
    display: inline-block;
    padding: 10px 20px;
    background-color: #007bff;
    color: white;
    text-decoration: none;
    border-radius: 4px;
    cursor: pointer;
}
```

---

## 📚 Related Documentation

- [README.md](README.md) - Project overview
- [ACTIVITIES.md](ACTIVITIES.md) - Activity documentation
- [LEARNING_PATH.md](LEARNING_PATH.md) - Learning guide
- [CONTRIBUTING.md](CONTRIBUTING.md) - Contribution guidelines

---

**Last Updated**: 2026-05-22

**Remember**: Consistency is more important than perfection. Follow these guidelines to maintain code quality and readability across the project.
