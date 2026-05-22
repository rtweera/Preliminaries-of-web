# HTML Activities - Detailed Documentation

This document provides comprehensive documentation for all HTML learning activities in this repository. Each activity builds on concepts from previous activities, creating a progressive learning path.

---

## 🎯 Activity 1: Basic HTML Structure

**File**: `HTML_Activity_01_215565L.html`

**Difficulty**: Beginner

**Duration**: 15-20 minutes

### 📚 Learning Objectives

- Understand the basic structure of an HTML document
- Learn about the DOCTYPE declaration
- Explore the purpose of `<head>` and `<body>` sections
- Work with common HTML elements (headers, paragraphs, images, links)
- Apply basic styling with HTML attributes

### 🔍 Key Concepts

#### HTML Document Structure
```html
<!DOCTYPE html>          <!-- Document type declaration -->
<html>                   <!-- Root element -->
    <head>              <!-- Metadata and document configuration -->
        <title>...</title>
    </head>
    <body>              <!-- Visible content -->
        ...
    </body>
</html>
```

#### Elements Used

| Element | Purpose | Example |
|---------|---------|---------|
| `<head>` | Contains metadata, title, scripts, styles | Sets page title and encoding |
| `<title>` | Page title shown in browser tab | "University of Moratuwa" |
| `<body>` | All visible page content | Main content goes here |
| `<header>` | Header section of the page | Page top with title and logo |
| `<h1>` | Main heading (largest) | Page heading |
| `<img>` | Embed images | University logo |
| `<p>` | Paragraph text | Body text and descriptions |
| `<a>` | Hyperlinks | Contact email link |
| `<footer>` | Footer section | Contact information |

### 💡 Key Features

1. **DOCTYPE Declaration**: `<!DOCTYPE html>` - Tells the browser this is an HTML5 document
2. **Body Background**: Uses `bgcolor="#fadadd"` attribute for pink background
3. **Image Integration**: External image from Wikipedia with proper alt text
4. **Email Links**: Uses `<a href="mailto:...">` for email functionality
5. **Semantic Structure**: Proper use of `<header>` and `<footer>` tags

### 📝 Practice Exercises

1. **Modify the title**: Change the `<title>` content and see it appear in the browser tab
2. **Change background color**: Try different color codes (e.g., `#ffffbf`, `#ffffff`)
3. **Add more paragraphs**: Insert additional `<p>` elements with your own content
4. **Add links**: Create links to other websites using `<a href="...">`
5. **Replace the image**: Change the image URL to another publicly available image

### ✅ Self-Check Questions

- [ ] What is the purpose of `<!DOCTYPE html>`?
- [ ] Where should page metadata go in an HTML document?
- [ ] How do you embed an image in HTML?
- [ ] What does the `alt` attribute do in an image tag?
- [ ] How do you create a clickable email link?

---

## 🎯 Activity 2: Semantic HTML & Lists

**File**: `HTML_Activity_02_215565L.html`

**Difficulty**: Beginner

**Duration**: 20-25 minutes

### 📚 Learning Objectives

- Understand semantic HTML and proper element usage
- Learn about different types of lists in HTML
- Explore the structure of definition lists
- Use text formatting elements properly
- Build organized content with semantic elements

### 🔍 Key Concepts

#### Semantic HTML

Semantic HTML uses meaningful tags that describe the content's purpose to both browsers and developers:

```html
<!-- Semantic (better) -->
<header>...</header>    <!-- Page header -->
<nav>...</nav>          <!-- Navigation -->
<section>...</section>  <!-- Content section -->
<article>...</article>  <!-- Article or post -->
<footer>...</footer>    <!-- Page footer -->

<!-- Non-semantic (less meaningful) -->
<div>...</div>          <!-- Generic container -->
<span>...</span>        <!-- Generic inline -->
```

#### Definition Lists

Definition lists (`<dl>`) are perfect for organizing term-definition pairs:

```html
<dl>
    <dt><b>Term</b></dt>           <!-- Definition Term -->
    <dd>Description of the term</dd> <!-- Definition Description -->
</dl>
```

This activity uses definition lists to organize university courses with their descriptions.

#### Text Formatting

| Element | Purpose | Example |
|---------|---------|---------|
| `<b>` | Bold text | `<b>Important</b>` |
| `<i>` | Italic text | `<i>Description</i>` |
| `<strong>` | Strong importance (semantic bold) | `<strong>Critical</strong>` |
| `<em>` | Emphasis (semantic italic) | `<em>Emphasized</em>` |

### 💡 Key Features

1. **Definition Lists**: Uses `<dl>`, `<dt>`, `<dd>` for course information
2. **Course Information**: Lists bachelor's programs with descriptions
3. **Text Formatting**: Combines `<b>` for course names and `<i>` for descriptions
4. **Yellow Background**: Uses `bgcolor="#ffffbf"` for visibility
5. **Header Structure**: Clear `<h2>` for "Undergraduate courses" section

### 📝 Practice Exercises

1. **Add new courses**: Insert additional `<dt>` and `<dd>` pairs for other programs
2. **Add postgraduate section**: Create a new section for master's degree programs
3. **Use semantic tags**: Replace `<b>` with `<strong>` and `<i>` with `<em>`
4. **Add hyperlinks**: Create links within descriptions to department websites
5. **Add nested content**: Create sub-lists within course descriptions

### ✅ Self-Check Questions

- [ ] What is the difference between semantic and non-semantic HTML?
- [ ] When should you use a definition list vs. an unordered list?
- [ ] What's the difference between `<b>` and `<strong>`?
- [ ] How are definition lists (`<dl>`) structured?
- [ ] Why is semantic HTML important for accessibility?

---

## 🎯 Activity 3: Layout & Image Positioning

**File**: `HTML_Activity_03_215565L.html`

**Difficulty**: Beginner-Intermediate

**Duration**: 20-25 minutes

### 📚 Learning Objectives

- Master image positioning and alignment
- Understand how HTML attributes control layout
- Learn to create more sophisticated page layouts
- Work with floated elements
- Improve visual hierarchy with positioning

### 🔍 Key Concepts

#### Image Attributes for Positioning

```html
<!-- Align attribute (deprecated but useful for learning) -->
<img src="..." alt="..." width="10%" align="right"/>

<!-- Width control -->
<img src="..." width="10%"/>       <!-- Percentage -->
<img src="..." width="100px"/>     <!-- Pixels -->

<!-- Alt text for accessibility -->
<img src="..." alt="Descriptive text"/>
```

**Note**: While `align` attribute is deprecated in modern HTML, understanding it helps learn layout concepts. Modern approaches use CSS.

#### Layout Concepts

1. **Float**: Positions image to the right, allowing text to flow around it
2. **Width Percentage**: Makes layout responsive to screen size
3. **Alt Text**: Provides description for screen readers and when images fail to load

### 💡 Key Features

1. **Right-Aligned Logo**: `align="right"` positions university logo to the right
2. **Responsive Width**: Uses percentage (`10%`) instead of fixed pixels
3. **Improved Accessibility**: Provides meaningful alt text for images
4. **Same Content Structure**: Uses the same definition list structure as Activity 2
5. **Better Visual Layout**: Logo doesn't interfere with content flow

### 📝 Practice Exercises

1. **Change image alignment**: Try `align="left"` or remove it to see the difference
2. **Adjust image size**: Change width from `10%` to `20%` or `5%`
3. **Experiment with positioning**: Add images in different locations on the page
4. **Test responsiveness**: Resize your browser to see how percentage-based sizing adapts
5. **Create image-text wrapping**: Add multiple paragraphs to see text flow around the image

### ✅ Self-Check Questions

- [ ] What does the `align` attribute do to an image?
- [ ] Why use percentage width instead of fixed pixels?
- [ ] What is the `alt` attribute and why is it important?
- [ ] How does right-aligning an image affect text layout?
- [ ] What happens when an image fails to load?

---

## 🎯 Activity 4: CSS Styling

**File**: `HTML_Activity_04_215565L.html`

**Difficulty**: Intermediate

**Duration**: 30-40 minutes

### 📚 Learning Objectives

- Learn internal CSS (stylesheets in `<style>` tag)
- Understand CSS selectors (element, ID, class)
- Style HTML elements with CSS properties
- Create complex layouts with CSS
- Build professional-looking web pages

### 🔍 Key Concepts

#### Internal CSS Structure

```html
<head>
    <style>
        /* CSS rules here */
        selector {
            property: value;
        }
    </style>
</head>
```

#### CSS Selectors

| Selector | Purpose | Example |
|----------|---------|---------|
| Element | Select all elements of type | `p { color: red; }` |
| ID | Select element with specific ID | `#header { ... }` |
| Class | Select elements with class | `.highlighted { ... }` |

#### Common CSS Properties

```css
body {
    padding: 10px;           /* Internal spacing */
    background-color: white; /* Background color */
    font-family: Arial;      /* Font choice */
}

#img-logo {
    float: left;            /* Float to left */
    width: 100px;           /* Fixed width */
}

ul, ol {
    list-style: none;       /* Remove bullet points */
}

table {
    border-collapse: collapse; /* Collapse table borders */
}
```

### 💡 Key Features

1. **Internal Stylesheet**: Uses `<style>` tag in `<head>`
2. **ID Selectors**: Targets specific elements like `#img-logo`
3. **Multiple Styling Rules**: Complex layout with floated elements
4. **Table Styling**: Comprehensive table formatting
5. **List Styling**: Custom styling for navigation lists
6. **Footer Layout**: Displays footer links inline

### 📝 Content: Hotel Green Stay Website

This activity creates a hotel website with:
- Hotel logo and information
- Room showcase with images and pricing
- Booking form
- Footer with contact information

### CSS Features Used

```css
/* Float layout */
#img-logo {
    float: left;
}

/* Centered table */
.centered-tbl {
    margin: 0 auto;
}

/* List styling */
#list-footer {
    list-style: none;
}

#list-footer li {
    display: inline;
    padding-right: 1rem;
}

/* Table styling */
table, th, td {
    border: 1px solid black;
}

th {
    background-color: green;
    color: white;
}
```

### 📝 Practice Exercises

1. **Change colors**: Modify background colors and text colors
2. **Adjust spacing**: Change padding and margins
3. **Create a new layout**: Reorganize where the logo appears
4. **Add more styles**: Create classes for different content sections
5. **Style the form**: Add CSS to make the form more visually appealing
6. **Create a navigation bar**: Style the header navigation with horizontal menu items
7. **Make it responsive**: Add media queries (advanced) for mobile devices

### ✅ Self-Check Questions

- [ ] What is the difference between internal and external CSS?
- [ ] What is CSS specificity and why does it matter?
- [ ] How do ID selectors differ from class selectors?
- [ ] What does the `float` property do?
- [ ] How do you center content on a page?
- [ ] What is the purpose of `border-collapse` in tables?
- [ ] How do you make inline lists in CSS?

---

## 📊 Comparison Table

| Feature | Activity 1 | Activity 2 | Activity 3 | Activity 4 |
|---------|-----------|-----------|-----------|-----------|
| HTML Structure | ✅ | ✅ | ✅ | ✅ |
| Semantic Elements | ✅ | ✅✅ | ✅✅ | ✅✅ |
| Lists | ❌ | ✅✅ | ✅✅ | ✅ |
| Images | ✅ | ❌ | ✅✅ | ✅ |
| CSS | ❌ | ❌ | ❌ | ✅✅ |
| Forms | ❌ | ❌ | ❌ | ✅ |
| Tables | ❌ | ❌ | ❌ | ✅ |

---

## 🚀 Progression Path

```
Activity 1: Basic HTML
    ↓ (Learn structure, elements, attributes)
Activity 2: Semantic HTML & Lists
    ↓ (Learn organization, semantic meaning)
Activity 3: Layout & Positioning
    ↓ (Learn visual organization)
Activity 4: CSS Styling
    ↓ (Learn professional styling)
    
→ Ready for intermediate web development!
```

---

## 🔗 Related Documentation

- [LEARNING_PATH.md](LEARNING_PATH.md) - Detailed learning progression guide
- [CODE_STYLE.md](CODE_STYLE.md) - Coding standards and best practices
- [RESOURCES.md](RESOURCES.md) - Additional learning resources

---

**Last Updated**: 2026-05-22
