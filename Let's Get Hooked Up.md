# Let's Get Hooked Up.

No Need to take the .js extension into the consideration here.

Hardcoded data should be kept in utils.js or constants.js inside the utils folder so that we have all the utilities files here and will be used all across our app.

There are two types of exports such as: Named Exports and Default Exports.

There can't be multiple default exports in a single file and import variable.

```javascript
    export default Header;
    import CDN_URL from '...';
```

Multiple exports can be done using Named Exports and export the variable and import variable.

```javascript
    export const fname="Aryan"
    import {CDN_URL} from '...';
```

We can also import and export the Component by using named exports and imports. We can use Default and Named Exports Together in the system.

React Hooks are basically normal JavaScript utility Functions.

Hooks Comprise Of: useState(), useEffect() etc. Hooks are imported as Named Imports. The method inside the useState is used to update the value of the state.

Whenever a state variable changes, react re-renders the component.

useState() - Superpowerful State Variables In React. 

Reconciliation is also called as React Fiber. This is called as the process when a virtual DOM changes when a part or component in the DOM is changed.

React creates a virtual DOM. Virtual DOM is a normal JavaScript object.

Diffing Algorithm finds difference between the Actual Virtual DOM and Updated Virtual DOM. React is faster due to Virtual DOM Concept.

Incremental rendering is used to render in the various of the chunks and contribute the thing in the form of small chunks and spread it over multiple chunks.
