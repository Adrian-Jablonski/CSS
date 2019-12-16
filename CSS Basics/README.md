# CSS Basics

## Helpful CSS Resources

- https://developer.mozilla.org/en-US/docs/Web/CSS
- https://webplatform.github.io/docs/css/
- https://www.w3.org/Style/CSS/Overview.en.html

## Importing stylesheets inside a css file

Add '@ import "import-styles.css";' to the top of the style.css stylesheet 

## CSS Data types

- https://wiki.developer.mozilla.org/en-US/docs/tag/CSS%20Data%20Type

## Shorthand Font property

```css
p {
    font-size: 1em;
    font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
    line-height: 1.5;
    
    /* The above three lines are equivalent to the below shorthand method */

    font: normal 1em/1.5 "Helvetica Neue", Helvetica, Arial, sans-serif;
}


```

## List item Nav

```css 
li {
    display: inline-block;
    padding: 0 12px;
    border-right: solid 1px;
    margin: 80px 0;
}

```