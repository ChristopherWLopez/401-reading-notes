# Class 27 Reading

## What was the motivation for introducing Hooks?

Hooks solve a wide variety of "unconnected problems"... React doesnt ofer a way to "attach" reusable behavior to a component. You can extract stateful logic from a component so it can be tested independently and reused. Hooks lets you reuse stateful logic without changing your component hierarchy.

## What changes are important regarding implementing Hooks versus Component Classes?

Changing es6 class components to Functional components.
you have to give up using `this` (which is great).

## Hooks allow you to reuse stateful logic without changing __________

without changing your component hierarchy.

## Name two rules imposed by React Hook usage

You can call hooks at the top level. Dont call hooks in loops conditions or nested functions.  

Only call hooks from react function components. Dont call from regular JS functions.

## How would you identify a custom Hook and why might you create one?

You would create them if you wanted to reuse some stateful logic between components

the convention is `use`.

## What is a Hook?

A Hook is a function that lets you use state without writing a class.
You are able to `hook` into react features `useState` lets you add React State to functional components. 

## When would I use the useState Hook?

Whenever you feel that the component you are workin on needs state.

## If you were to add React state to a function component by declaring a state variable:

### What does calling useState do?

It declares a state variable. This is a way to preserve some value between functions.

### What do we pass to useState as an argument?

The initial state. this doesnt Have to be an object, although it Can be... we just need to initial value.

### What does useState return?

It returns a pair, this is the state we are updating and the function that updates it.

## What are your learning goals after reading and reviewing the class README?

To get a better understanding of functional components. And hopefully other state hooks.

## overall notes

useEffect alows us the ability to perform side effects with functional components.
