# Javascript Drum Kit

## What I Learnt?

### HTML and CSS:

- `data-*` : This attribute is a global attribute and can be applied on any HTML element. This attribute helps us in storing custom data private to page or application and also enables us to embed data attribute on all HTML elements.
  - In this exercise we hooked up `data-key` with `audio` attribute. When someone hits a key on the keyboard we gonna find a corresponding audio element and play it
- `<kbd>` : Keyboard Input element
- `audio` : `audio` tag is used to embed sound content on your webpage.
- `transition` :transitions make the element smoothly and gradually change from one state to another.
- `transform` : transforms move or change the appearance of an element from one state to another.
- [Transition and transform](https://thoughtbot.com/blog/transitions-and-transforms#:~:text=So%20what%20are%20transforms%20and,from%20one%20state%20to%20another.)

### Javascript:

- `audio.play()` : plays the associated sound from the audio tag.
- `audio.currentTime = 0` : rewinds the song to the starting of it
- `transitionend event` : You can remove a transition on an element by using this event instead of using `setTimeOut` to remove a classList on an event
- ```js
  const keys = document.querySelectorAll(".key");
  keys.forEach((key) =>
    key.addEventListener("transitionend", removeTransition)
  );
  const removeTransition = (e) => {
    // some logic goes here to remove transition.
  };
  ```
- `Array.from()` -[MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/from): > The Array.from() static method creates a new, shallow-copied Array instance from an array-like or iterable object.
