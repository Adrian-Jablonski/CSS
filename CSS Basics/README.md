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

## Text shadow

```css 

h1 {
    /* The first value sets the horizontal offset of the shadow. 
    The second value sets the vertical offset. 
    The third is an optional value that sets the blur radius of the shadow. 
    The fourth value is the color value. */
    text-shadow: 5px 8px 10px #222;
}

```

## Box Shadow

```css 

div {
    /* 20px spreads shadow on every side of div */
    box-shadow: 15px 15px 10px 20px rgba(0, 0, 0, .8);

    box-shadow: inset 0 0 50px 10px rgba(0, 0, 0, 1); /* Inset moves the shadow to the inside of the div */
}

```

## Gradients

```css
div {
    background-image: linear-gradient(45deg, #ffa949, firebrick);

    background-image: radial-gradient(circle, #ffa949, firebrick);

    /* Gradient Color Stops */
    background-image: linear-gradient(45deg, #ffa949 0%, firebrick 50%, dodgerblue 100%);
}
```

## Multiple Background and Transparent Gradients

```css
div {
    background: linear-gradient(#ffa949, transparent 90%)   /* Overlays a transparent background on the background image below */
                #ffa949 url('../img/mountains.jpg') no-repeat center;
}

```

## Web Fonts

```css 
@font-face {
    font-family: 'Abolition Regular';
    src: url('../fonts/abolition-regular-webfont.eot'); /* file path is to a font file saved in fonts folder */
}

h1 {
    /* Using the font that was set in @font-face by font-family name */
    font-family: 'Abolition Regular', Helvetica, Arial;
}

```

## Media queries

```css
@media (max-width: 960px) { /* Targets anything at or below 960px */ 
    body {
        background: blue;
    }
    p {
        color: white;
    }
}

@media (min-width: 481px) and (max-width: 700px) { /* Targets anything between 481px and 700px */ 

}

```