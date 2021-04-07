# JS + CSS Clock

## What I Learnt?

### CSS:

We need to rotate the hand based on the time in the PC.

- `transform` :
  > From [CSS Tricks](https://css-tricks.com/almanac/properties/t/transform/): The `transform` property allows you to visually manipulate an element by skewing, rotating, translating, or scaling

```css
transform: rotate(20deg);
```

`transform` by default rotates itself on the exact middle of the element. In this application we dont want that to happen, we want to rotate it towards the right hand side of thw application.
we use `transform-origin` for that.

```css
 transform-origin = 100% /*The center point would be at the right end of the hand*/
```

> From [CSS Tricks](https://css-tricks.com/almanac/properties/t/transform-origin/): The transform-origin property is used in conjunction with CSS transforms, letting you change the point of origin of a transform.

---

Our divs are from left to right. Initially hands position will be at 9 o clock, to get it at 12 0 clock,

```css
transform: rotate(90deg);
```

`transition` : to have a smooth animation over the time period.
[Using CSS Transitions](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Transitions/Using_CSS_transitions)
