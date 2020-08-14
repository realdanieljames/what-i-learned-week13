# [Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

## can find a full run down of the css flex-box properties and rules [here](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
```css
.container {
  display:flex /* or inline-flex */
}
```
- flexbox is model for laying out content in a given box.
- its a more efficient way to lay out, align and distribute space among items in a container. 

### container properties
### flex-direction
- This establishes the main-axis, thus defining the direction flex items are placed in the flex container.
  
```css
  .container {
  flex-direction: row | row-reverse | column | column-reverse;
}
```

- justify-content
### flex-wrap
- By default, flex items will all try to fit onto one line. You can change that and allow the items to wrap as needed with this property.
- 
```css
  .container {
  flex-wrap: nowrap | wrap | wrap-reverse;
}
```

<hr>

- align-items
- align-content

100vh; viewport height
100vw; viewport weight
- however tall 

holy grail layoutt
<hr>
<hr>

## Emmet Abbreviation

- auto completes html doc, tags, etc.
- [Emmet Cheatsheet](https://docs.emmet.io/cheat-sheet/)
   <!-- div.container>div.square#item${ITEM $}*8 -->

* `<div>`s by default takes up the whole row.
<hr>
<hr>


## media queries
* It uses the @media rule to include a block of CSS properties only if a certain condition is true.
* mobile responsiveness

max-width (at most)(maximum)
min-width (at least)(minimum)
orientation: landscape
orientation: portrait

## media queries Example
```css
/* this is a new rule that applies in certain circumstances */
/* at maximum 600 pixels */
/* this rule applies */
@media (max-width: 600px) {
  .square {
    background-color: black;
  }
}

@media (max-width: 400px) {
  .square {
    background-color: 5px solid purple;
  }
}
```
* mobile first development (assume the user is on a phone)

<hr>
<hr>

# [CSS GRID](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout) 

-CSS Grid Layout excels at dividing a page into major regions or defining the relationship in terms of size, position, and layer, between parts of a control built from HTML primitives.


### display: grid;

### grid-template-columns:
### grid-template-rows:
### grid-template-areas:




```css
.app {
  display: grid;
  width: 300px;
  height: 300px;
  /* grid-template-rows: 1fr 1fr 1fr ;
  grid-template-columns: 1fr 1fr 1fr; */
  grid-template-rows: 1fr 1fr 1fr ;
  grid-template-columns: 1fr 1fr 1fr;
}

.square {
 
  background-color: blue;
  border: 3px solid green;
}


#upper-left {
  grid-row: 1 / 3; // this should go from row line1, to row line 3
  grid-column: 1 / 2; // column line1 to column line2
}

```

- grid is good for bigger scale applications
- space separated list (array of values)
- fractions (fr) sized by even fractions or by using percentages.
- spans can be useful for moving things around the grid also. 

```css
#map {
grid-column: 2 / span 2; // start at column 2 and span(stretch) 2 columns over.
grid-row: 1 / span 3; // start at first row and span(stretch) 3 rows over.
}
```

# grid-template-areas: 
- helps to identify areas of the grid
- every string in quotes is a row
- uses 3 character words to represent 
- a 2d array
  
<hr>
<hr>

## Arrow functions



```javascript
const add = (x, y) =>  x + y;



const add = function (x, y) {
  return x + y;


  const sayHi = () => cosole.log('hi');

  const add5 = (n) => n + 5; // better practice 
  const add5 = n => n + 5;  // does not need parentheses if only parameter
}
```

