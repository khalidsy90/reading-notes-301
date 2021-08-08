# React lifecycle

**1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?**

**Arrangement Mounting lifecycle methods**

    - constructor()
    - static getDerivedStateFromProps()
    - render()
    - componentDidMount()

**2. What is the very first thing to happen in the lifecycle of React?**

The normal thing is when Class is called, the first thing that will work is the constructor

**3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates**

    - constructor
    - render
    - componentDidMount
    - React Updates
    - componentWillUnmount

---

# React State & Props

**1. What types of things can you pass in the props?**

The values can be any data type, from strings to functions, objects, etc.

**2. What is the big difference between props and state ?**

**State** is the local state of the component which cannot be accessed and modified outside of the component. It's equivalent to local variables in a function.

JS Function

```javascript
const DummyFunction = () => {
  let name = "Manoj";
  console.log(`Hey ${name}`);
};
```

React Component

```javascript
class DummyComponent extends React.Component {
  state = {
    name: 'Manoj'
  }
  render() {
    return <div>Hello {this.state.name}</div>;
  }
```

**Props**, on the other hand, make components reusable by giving components the ability to receive data from their parent component in the form of props. They are equivalent to function parameters.

Plain JS Function

```javascript
const DummyFunction = (name) => {
  console.log(`Hey ${name}`);
};
```

// when using the function

```javascript
DummyFunction("Manoj");
DummyFunction("Ajay");
```

React Component

```javascript
class DummyComponent extends React.Component {
render() {
return <div>Hello {this.props.name}</div>;
}

}

// when using the component
<DummyComponent name="Manoj" />
<DummyComponent name="Ajay" />
```

### Changing props and state

```
                                                   props   state
    Can get initial value from parent Component?    Yes     Yes
    Can be changed by parent Component?             Yes     No
    Can set default values inside Component?*       Yes     Yes
    Can change inside Component?                    No      Yes
    Can set initial value for child Components?     Yes     Yes
    Can change in child Components?                 Yes     No
```

**3. When do we re-render our application?**

whenever there is a change in their state or props

**4. What are some examples of things that we could store in state?**

we can use it with objects,arrays,colors,properties

## Things I want to know more about

1. When can I actually use state and how can I update it without problems?

2. How do I deal with the state with the hooks or without the hooks?
