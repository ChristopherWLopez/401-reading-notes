# Class 29 Reading notes

## What purpose does useEffect serve in a function component compared to its counterpart(s) in class components?

`componentDidMount` , `componentWillMount`, and `componentDidUpdate`

## When using the useEffect Hook

### What does useEffect do?

- useEffect takes ina function that is run AFTER the DOM is updated.

### Why is useEffect called inside a component?

- This allows us access to the count state variable, from the effect. This does not require any API to read it. This also embraces JS's closures.

## Explain the importance of properly implementing effects with Cleanup

It is important to clean up so we dont "introduce a memory leak". When using hooks this allows us from repeating the code (much like we would with `componentDidount` and `componentWillMount` etc...). Also for the sake of readibility we are able to keep code DRY.

React will clean up before the next re-render.

## Things I want to know more about

- I think I am missing something here. I may need to know more about this topic of `useEffect` and or I am missing a piece of the `lifeCycle` topic. So in short.... I want just want to know more about these topics. 