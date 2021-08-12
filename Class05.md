**How would you break a mock into a component heirarchy**

draw boxes around every component (and subcomponent) in the mock and give them all names. If you’re working with a designer, they may have already done this

**What is the single responsibility principle and how does it apply to components**

a component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.

**What are the three questions you can ask to determine if something is state?**
Is it passed in from a parent via props? If so, it probably isn’t state.
Does it remain unchanged over time? If so, it probably isn’t state.
Can you compute it based on any other state or props in your component? If so, it isn’t state

**What does it mean to build a ‘static’ version of your application**

use mock data, and pass those down as props to other components as I build out the app. For example, lets look at a real component I will be building, called "Patients". Ignore the JSON format, it will be in regular JS object notation in the real app.

**How can you identify where state needs to live?**

if my component depends on a data to render and show some results, then this data can be placed in state. State changes, component rerenders and show results depending on the state.

**What does it mean to build a ‘static’ version of your application?**

The easiest way is to build a version that takes your data model and renders the UI but has no interactivity. To build a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props.
