# Playing with CSS Variables and JS

## Things I Learnt

### HTML and CSS

- `input type = 'color'` : gives us color picker

#### CSS Variables

- `:root` - A pseudoclass which applies custom properties of CSS globally(across the html document).
- `var()` - Using var() you can call the custom css property in your element

- More about [CSS variables from MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties)

### JS

- `this.dataset` : contains all the data attributes of html element in this object
- `document.documentElement` : Gets the root element of html document
  > [MDN Docs](https://developer.mozilla.org/en-US/docs/Web/API/Document/documentElement)
- To set a css value to an element
  ```js
  document.documentElement.style.setProperty("--var_name", "value");
  ```
- [Set and Get CSS variable values in JS](https://davidwalsh.name/css-variables-javascript)
