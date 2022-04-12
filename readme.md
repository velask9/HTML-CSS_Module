# HTML & CSS
Reference project that illustrates HTML, CSS, Flexbox and Bootstrap. Assignments are located [here](./assignments.md).

# Getting Started
- Install VSCode 
- Install VSCode extension: Live Server
- Clone this repo:
  - Make a directory on your computer
  - CD into this directory
  - Execute: `git clone git@github.com:mburolla/html-css.git` 
- Right click on `index.html` and "Open with Live Server"

# Videos
- [Types of Web Architectures 10m](https://youtu.be/Qms4k6y7OgI)
- [PluralSight HTML Fundamentals 2h 20m](https://app.pluralsight.com/course-player?clipId=ecbf549b-e454-4d5a-9872-367356892b14)
- [HTML and CSS Tutorial 2h 17m](https://youtu.be/D-h8L5hgW-w)
- [CSS Specificity Explained 13m](https://youtu.be/c0kfcP_nD9E)
- [CSS Positioning 1hr](https://app.pluralsight.com/library/courses/css-positioning-1834/table-of-contents)
- [Modern Web Layout with Flexbox and CSS Grid 1h 10m](https://app.pluralsight.com/library/courses/modern-web-layout-flexbox-css-grid/table-of-contents)
- [Flexbox Crash Course 2022 46m ](https://youtu.be/3YW65K6LcIA)
- [Bootstrap 5 Grid System Tutorial 15m](https://youtu.be/DZKf9l42WCo)
- [Getting Started with Bootstrap 5 1h](https://youtu.be/1nxSE0R27Gg)

# Links
- [Flexbox helper page](flex-index.html)
- [Bootstrap helper page](bs-index.html)
- [W3Schools](https://www.w3schools.com/)
- [Bootstrap flex](https://getbootstrap.com/docs/4.0/utilities/flex/)
- [Bootstrap Utilities](https://getbootstrap.com/docs/4.0/utilities/borders/)
- [Common CSS Properties](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Properties_Reference)
- [Specificity](https://www.w3schools.com/css/css_specificity.asp)
- [HTML Semantic Elements](https://www.w3schools.com/html/html5_semantic_elements.asp)

# How to Learn
What Will This Do (WWTD)?  This is a game you can play on your own to help you learn style and layout.  Try to visualize what will happen BEFORE you make a change to something.  For example:

How will the display change when 10px is changed to 20px?
```
body {
    padding: 10px; /* WWTD */
}
```

# Notes
HTML HyperText Markup Language is used to create Web pages and tells the browser how to display them. The purpose of CSS is to provide Web developers with a standard way to define, apply, and manage sets of style characteristics.  In other words, HTML is the data and CSS is the style.  Keeping these tasks separate is an architectual style known as the separation of concerns.

### HTML Semantic Elements
A semantic element clearly describes its meaning to both the browser and the developer. Examples of non-semantic elements (tells nothing about the content):
``` 
<div>
<span>
```

Examples of semantic elements (Clearly defines its content): 
```
<form>
<table>
<article>
```

HTML elements that could possibly be used by SEO:
```
<header>
<nav>
<main>
<footer>
```

# CSS
Four important concepts:
- Box Model
- CSS Selectors
- Specificity
- Positioning

### Box Model
- DevTools >> Elements Tab >> Scroll all the way down & click on HTML elements on left
- Margin: Outside of the HTML element
- Border: Actual border of the HTML element (the fence?)
- Padding: inside of the HTML element

### CSS Selectors
These CSS selectors are used to target HTML elements so that they can be styled:

|Example            |Description                          |
|-------------------|-------------------------------------|
|`* {}`             |Universal Selector                   |
|`body {}`          |General Selector                     |
|`#menu {}`         |ID Selector                          |
|`.bookTitle {}`    |Class Selector                       |
|`div p {}`         |Descendant Selector (match any level)|
|`div > p {}`       |Child Selector (match specifically)  |
|`img[alt=check] {}`|Attribute Selector                   |
|`a:visited {}`     |Psuedo Selector                      |

NOTE: Targeting specific HTML elements in a React App is easier because we can leverage Sassy CSS (Sass) and CSS modules.

### Specificity
Specificity is the means by which browsers decide which CSS property values are the most relevant to an element and, therefore, will be applied.  In other words, specificity determines what rule sets will be applied to a target element. 

### Positioning
Note: Block, Inline, Table and Positioning are old techniques that do not provide the flexibility that we need in today's world.

- Fixed: Permanently located with respect to browser window, does not scroll bar (taken out of document flow).
- Absolute: Like Fixed positioning, but responds to scroll bar (taken out of document flow).
- Relative: Relative to its original position in the document flow.
- Static: Disables positioning values, does not move the element (default value for all elements).
- Inherit: Inherit the position from the parent container element.
- Z-index: Higher numbers stack elements on top of each other.

---

The key concept to understand when using flexbox is that there are two classes associated with "flexing", the flex container itself, and the actual item(s) inside the container.  There are properties ONLY associated with the flex container and ONLY associated with the flex item(s).  The definitions of "main axis" and "cross axis" must be undertood.  Flexbox works with block elements.

#### Flexbox Container Props
These properties ONLY apply to the flexbox container. Default direction is left-to-right (row), this is the main axis, the cross axis is 90 degrees from th main axis.

- `display`: {flex|inline-flex} Inline shrink wraps flexbox items
- `flex-direction`: {column|row} Row is the default
- `flex-wrap`: Used to specify if the flex container should wrap flex items and not squish items (squish is default)
- `flex-flow`: Shorthand for flex-direction and flex-wrap
- `justify-content`: {first baseline|center|space-between} along the main axis
- `align-items`: {flex-start|center|flex-end} Aligns the flexbox items across the CROSS axis
- `align-content`: Applies alignment accross the CROSS axis for items that wrap multiple lines (does nothing for single line flex containers) stretch is default
- `gap`: Space between flexbox items

#### Flexbox Item Props
These properties ONLY apply to the flex item(s):
- `order`: The order in which to render the flex item
- `flex-grow`: How much an item will GROW relative to the rest of the flexible items inside the same container
- `flex-shrink`: How much an item will SHRINK relative to the rest of the flexible items inside the same container
- `flex-basis`: The initial length of a flexible item 
- `flex`: Shorthand for: `flex-grow` `flex-shrink` `flex-basis`
- `align-self`: Individually change [alignment](https://getbootstrap.com/docs/5.1/utilities/flex/#align-self) for flexbox items on the cross axis, including stretch

---

# Bootstrap 
The Bootstrap grid system (rows & columns) contains 12 column units.  Bootstrap stacks divs verticall only if one or more of the responsive breakpoints (class infix) have been hit.

To include Bootstrap in your webpage, add the following references to the `<head>` tag:
```
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p" crossorigin="anonymous"></script>
```

# Responsive Breakpoints
A responsive breakpoint is "hit" when the browser is expanded to the width specified in this table:

|Breakpoint       |Class infix  |Width      |
|-----------------|-------------|-----------|
|X-Small          |None         |0-575px    |
|Small            |sm           |>=576px    |
|Medium           |md           |>=768px    |
|Large            |lg           |>=992px    |
|Extra Large      |xl           |>=1200px   |
|Extra extra large|xxl          |>=1400px   |

ProTip: To view the width of the browser ensure that the Dev Tools console is open (Ctl+Shift+i) and observe the dimensions in the upper right hand corner of the browser window.

