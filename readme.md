# HTML CSS
Reference project to illustrate HTML & CSS.

# Assignments
[Assignments](./assignments.md)

# Getting Started
- Clone this repo
- Install Live Server extension (VSCode)
- Right click on `index.html` and "Open with Live Server"

# Notes
HTML HyperText Markup Language is used to create Web pages and tells the browser how to display them. The purpose of CSS is to provide Web developers with a standard way to define, apply, and manage sets of style characteristics.  In other words, HTML is the data and CSS is the style.  Keeping these tasks separate is an architectual style known as the separation of concerns.

# Resources
- [W3Schools](https://www.w3schools.com/)

# HTML
- [PluralSigth HTML Fundamentals](https://app.pluralsight.com/course-player?clipId=ecbf549b-e454-4d5a-9872-367356892b14)

### HTML Semantic Elements
[HTML Semantic Elements](https://www.w3schools.com/html/html5_semantic_elements.asp)
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
Three important concepts:
- Box Model
- CSS Selectors
- Specificity

### Box Model
- DevTools >> Elements Tab >> Scroll all the way down & click on HTML elements on left
- Margin: Outside of the HTML element
- Border: Actual border of the HTML element
- Padding: inside of the HTML element

### CSS Selectors
These CSS selectors are used to target HTML elements so that they can be styled:

|Example|Description|
|-----------|-----------|
|`* {}`|Global|
|`body {}`|General|
|`#menu {}`|ID|
|`.bookTitle {}`|Class|
|`div p {}`|Descendant (match any level)|
|`div > p {}`|Child (match specifically)|
|`img[alt=check] {}`|Attribute|
|`a:visited {}`|Psuedo|

NOTE: Targeting specific HTML elements in a React App is easier because we can leverage Sassy CSS (Sass) and CSS modules.

### Specificity
Specificity is the means by which browsers decide which CSS property values are the most relevant to an element and, therefore, will be applied.  In other words, specificity determines what rule sets will be applied to a target element. ProTip: Avoid `!important`
[Specificity](https://www.w3schools.com/css/css_specificity.asp)
[CSS Specificity Explained](https://youtu.be/c0kfcP_nD9E)

# How to Learn
What Will This Do (WWTD)?  This is a game you can play on your own to help you learn style and layout.  Try to visualize what will happen BEFORE you make a change to something.  

Example:
How will the display change when 10px is changed to 20px?
```
body {
    padding: 10px; /* WWTD */
}
```
