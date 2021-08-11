**What is a ‘Controlled Component’?**

Controlled Component is one that takes its current value through props and notifies changes through callbacks like onChange. A parent component "controls" it by handling the callback and managing its own state and passing the new values as props to the controlled component. You could also call this a "dumb component".

**Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.**

HTML form submission works differently when implementing it within a React.js component. Normally, the browser would render the HTML and, depending on the action, automatically submit the data of the form based on each element's name attribute. Although this default behavior still works in React.js, it is highly advised to programmatically submit a form by supplying your own custom controls on how data is processed by a component.

**How do we target what the user is entering if we have an event handler on an input field?**

using three keyboard events:

onKeyDown
onKeyUp
onKeyPress
These events are triggered when users touch, release, or hold keys, and they are used to to process specific user input.

**Why would we use a ternary operator**

The ternary operator greatly increases the conciseness of your code. When it is formatted correctly it can also be very easy to read and, dare I say it, even easier then if-else statements.

```javascript
x === y ? console.log(true) : console.log(true);
```

## Things I want to know more about

I want to know more about React Hooks
