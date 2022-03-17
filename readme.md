# HTML CSS
Reference project to illustrate HTML & CSS.

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
Two important concepts:
- Box Model
- CSS Selectors

### Box Model
- DevTools >> Elements Tab >> Scroll all the way down & click on HTML elements on left
- Margin: Outside of the HTML element
- Border: Actual border of the HTML element
- Padding: inside of the HTML element

### Selectors
These CSS selectors are used to target HTML elements so that they can be styled:

|Example|Description|
|-----------|-----------|
|`body {}`|General|
|`#menu {}`|ID|
|`.bookTitle {}`|Class|
|`div p {}`|Descendant (match any level)|
|`div > p {}`|Child (match specifically) |
|`img[alt=spacer] {}`|Attribute|
|`a:visited {}`|Psuedo|
|`* {}`|All|


# How to Learn
What Will This Do (WWTD)?  This is a game you can play on your own to help you learn frontend development.  Try to visualize what will happen before you make a change to something.  Example:
```
body {
    padding: 10px; /* WWTD */
}
```
