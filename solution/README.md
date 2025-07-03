<h1>
  <span class="headline">Intro to CSS</span>
  <span class="subhead">Solution</span>
</h1>

If you need to check your work, the full solution code can be found here.

HTML
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="./style.css">
    <title>Intro to CSS</title>
</head>
<body>
    <h1>Intro to CSS</h1>
    <p id="about">More About CSS</p>
    <div>This is a DIV</div>
    <div class="important">This is another DIV</div>
    <div class="important super-cool">
        <div>
            <p>Double nested</p>
        </div>
      <p>This is a paragraph inside of the third DIV</p>
    </div>
    <a href="https://github.com">Visit GitHub</a>
    <div id="comments">
      <h2>Comments</h2>
      <ul>
        <li>Comment One</li>
        <li class="super-cool">Comment Two</li>
      </ul>
      <button>This button does nothing</button>
    </div>
    <footer>Here's a footer</footer>
  </body>
</html>
```

CSS
```css
body {
    margin: 0;
    color: lightgrey;
    --brand-color: #91b8c4;
}

ul {
    margin: 0;
}

div {
    color: blue;
}

h1 {
    /* color: var(--brand-color); */
    text-align: justify;
    font-size: 28px;
    font-family: Arial, Helvetica, sans-serif;
    font-weight: 900;
    font-style: italic;
    text-align: center;

}

#about {
    font-style: italic;
    color: hotpink;
}

p {
    /* color: var(--brand-color); comment */
    /* padding-bottom: 7px;
    padding-left: 2px;
    padding-right: 3px;
    padding-top: 4px; */
    padding: 4px 3px 7px 2px;
    border: 2px;
    border-style: solid;
    border-color: red;
    margin-top: 10px;
}

.important, p, h1, .super-cool {
    color: var(--brand-color)!important;
}

.important p {
    color: green;
}

.super-cool {

    border: 2px solid pink;
}
```
