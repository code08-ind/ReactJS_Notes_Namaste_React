# Hooks

## useMemo Hook

It is used to cache the results between the re-renders.

Remove the strict mode otherwise it will be called twice. In production it won't happen and will be called only once. This strict mode will be found inside the index.js file.

If the code is not written properly, sometimes code gets mixed up here.

We can memoize the heavy operation here.

useMemo hook takes function which needs to be memoized or the value it returns as its first param. useMemo returns the value as it returns the result between re-renders and it also takes dependencies for which we do not need to memoize it sometimes and until dependencies changes, cache my result.

## useCallback Hook

It is used to cache a function definition between re-renders.

const myCallback = useCallback(func, [deps]);

## useRef Hook

It is used to store the reference of the DOM element that is not needed for rendering even if the component is rendered using some variable out here.

If the component is re-rendered again, all the normal vars will be set to the default value but the ref will not be set to the default value.

ref in useRef is something similar to being an object here. It has a property called as current that is the current value we pass to that variable. 

To print the current value, i will use the ref.current here.

If we have to update the ref variables, that can be done similar as we increase a normal variable. eg: ref.current = ref.current + 1;

When we again re-render the component, the ref still persists the value and then it updates the value there.



