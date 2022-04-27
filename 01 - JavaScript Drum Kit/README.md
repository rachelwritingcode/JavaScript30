## JavaScript 30 - Day 1: What Did I Learn? 🍎
---
### Template Literals

- Template literals are literals delimited with backtick (`) characters, allowing for multi-line strings, for string interpolation with embedded expressions, and for special constructs called tagged templates.

---
### String Interpolation 

- Template literals provide an easy way to interpolate variables and expressions into strings.The method is called string interpolation.

```
// String Interpolation
let firstName = "Jade";
let lastName = "Rabbit";
let text = `Welcome ${firstName}, ${lastName}!`; 

// Multi-line comment 
console.log(`string text line 1
string text line 2`);
```
---
### Tagged Templates 

- A more advanced form of template literals are tagged templates.
- Tags allow you to parse template literals with a function. The first argument of a tag function contains an array of string values. The remaining arguments are related to the expressions. 


[Reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals#tagged_templates)

---
### Events
- Events are actions or occurrences that happen in the system you are programming — the system produces (or "fires") a signal of some kind when an event occurs, and provides a mechanism by which an action can be automatically taken (that is, some code running) when the event occurs. 
- JavaScript lets you execute code when events are detected.

Example: When the click event is triggered, the background colour is changed.
```
btn.addEventListener('click', () => {
  const rndCol = `rgb(${random(255)}, ${random(255)}, ${random(255)})`;
  document.body.style.backgroundColor = rndCol;
});

```
[Reference](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)

---
### Array Object
Array Object - forEach

forEach() method executes a provided function once for each array element.
In the example, for each key pressed, the event listener function will run when the key press event is fired.

```
const keys = Array.from(document.querySelectorAll('.key'));
keys.forEach(key => key.addEventListener('transitionend', removeTransition))
window.addEventListener('keydown', playSound);
```

---
### HTML Transition End Event

`HTMLElement: transitionend event`
- The transitionend event is fired when a CSS transition has completed. In the case where a transition is removed before completion, such as if the transition-property is removed or display is set to none, then the event will not be generated.


```
const transition = document.querySelector('.transition');

transition.addEventListener('transitionend', () => {
  console.log('Transition ended');
});

```
[Reference](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement/transitionend_event)