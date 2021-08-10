**What does .map() return?**

A new array with each element being the result of the callback function.

**If I want to loop through an array and display each value in JSX, how do I do that in React?**

by using map function

**Each list item needs a unique key**

**What is the purpose of a key?**
to track if there were any changes made

**What is the spread operator?**
refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.

**List 3 things that the spread operator can do.**

1. Copying an array
2. Inserting the elements of one array into another
3. Array to arguments

**Give an example of using the spread operator to combine two arrays.**

```
let arrs = [[1, 2], [3, 4], [5, 6]];
arrs.reduce((a, b) => [...a, ...b], []);
```

**Give an example of using the spread operator to add a new item to an array.**

```
let a = [1, 2, 3, 4, 5];
let b = [0, ...a];
```

**Give an example of using the spread operator to combine two objects into one.**

```
let person = {
firstName: 'khalid',
lastName: 'hamedi',
age: 25,
ssn: '123-456-2356'
};

let job = {
jobTitle: 'JavaScript Developer',
location: 'USA'
};

let employee = {
...person,
...job
};
```

**In the video, what is the first step that the developer does to pass functions between components?**

Parent components pass props down to its children. Children components can not pass props up to their parent component.

**In your own words, what does the increment function do?**

update state of component

**How can you pass a method from a parent component into a child component?**

Passing method as a prop using the arrow function

**How does the child component invoke a method that was passed to it from a parent component?**
by using props

## Things I want to know more about

how to use getDerivedStateFromProps()
