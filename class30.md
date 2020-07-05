# Hooks api

Hooks are a new addition in React 16.8. They let you use state and other React features without writing a class.

## useState

``` const [state, setState] = useState(initialState); ```
Returns a stateful value, and a function to update it.

During the initial render, the returned state (state) is the same as the value passed as the first argument (initialState).

The setState function is used to update the state. It accepts a new state value and enqueues a re-render of the component.

## Functional updates

If the new state is computed using the previous state, you can pass a function to setState. The function will receive the previous value, and return an updated value. Here’s an example of a counter component that uses both forms of setState

## Lazy initial state

The initialState argument is the state used during the initial render. In subsequent renders, it is disregarded. If the initial state is the result of an expensive computation, you may provide a function instead, which will be executed only on the initial render

```const [state, setState] = useState(() => {
  const initialState = someExpensiveComputation(props);
  return initialState;
});
```

## useEffect

accepts a function that contains imperative, possibly effectful code.