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

## Box sizing

```css 
div {
    width: 960px;
    padding-left: 50px;
    padding-right: 50px;
    box-sizing: border-box; /* Box sizing will keep the size of the div at 960px and will not add 100px to that value from the padding */
}

* {
    box-sizing: border-box; /* Setting box-sizing to border-box using the universal selector will save us from writing it multiple times on multiple elements */
}

```

## Max width on image

```css 
img {
    max-width: 100% /* Makes image adjust to screen size */
}
```

## Background images

```css 
.image {
    background-color: #ffa949;
    background-image: url('../img/image1.png');
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;

    background: #ffa949 url('../img/imgage1.png') no-repeat center / cover; /* Shorthand background property */
}
```

## Floats

```html
<div class="group">
    <div class="col-1">
    
    </div>
    <div class="col-2">
    
    </div>

</div>

```

```css 
.col-1,
.col-2 {
    width: 46.5%;
}

.col-1 {
    float: left;
}

.col-2 {
    float: right;
}

/* Float Clearfix - Fixed the divs that were collapsed when using float ---------- */
.group:after {
    content: "";
    display: table;
    clear: both;
}

```