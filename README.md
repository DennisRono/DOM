# Document Object Model (DOM)

DOM - it is an interface that treats an HTML document as a tree like structure where each node is an object representing part of the document.

## How The DOM is Created

The DOM is created when the page loads from the HTML/CSS/JavaScript that the web server provides to the browser.

creating a DOM structure involves **creating individual nodes and organizing them in a hierarchical structure.**

## DOM Manipulation

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <h1 class="title">This is a TITLE</h1>

    <button class="btn">Remove Title</button>
    <script src="./index.js"></script>
  </body>
</html>
```

```jsx
const btn = document.querySelector('.btn')

btn.addEventListener('click', () => {
  const title = document.querySelector('.title')
  title.remove()
})
```

# how the DOM works as a tree

Tree is a metaphor to explain the DOM because everyone has likely seen a tree.

The DOM Works Like a Tree with the root at the Top branching downwards, with nodes nested inside each other.

```html
body / \ div div / \ p p / \ "Hi!" "Bye!"
```

## Creating and Inserting DOM nodes

to create a DOM node we use `document.createElement()`

## Adding Elements to the DOM

we use `append()`, `innerHTML`

## Changing Element Properties

```jsx
const element = document.getElementById('main')
element.style.backgroundColor = '#27647B'
```

## **Remove Elements from the DOM**

to remove elements we use **`removeChild()`** and **`remove()`**
