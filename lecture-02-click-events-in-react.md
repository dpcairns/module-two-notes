# Lecture 02 - Click Events in React

## React debugging
- Keep the console open. React errors are useful but sometimes dense and overwhelmingly wordy.
- The classic: if you see the word 'adjacent' in the error message, check to see if you're returning more than one parent element from a component.
- React components need a unique 'key' when you .map
- Track the props from top to bottom. Is the chain broken?
- Console.log/breakpoint props and state in the 'cool zone'. 
    - Did you get the props you expected from the parent? 
    - Did you get the state you expected from? 
- Be careful with click listeners! Did you remember to use the arrow syntax? 
    - `<div onClick={() => setItem(6)}>` works  
    - `<div onClick={setItem(6)}>` creates an infinite loop

## Pushing immutable to arrays

```js
const newArray = [...oldArray, newItem]

setArrayInState(newArray)
```

## From Scratch Demo: Cookie Clicker

## Half-Baked Project: Busy Town