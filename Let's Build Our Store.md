# Let's Build Our Store

We also have other libraries that manage our state safely. Eg: Zustand, Recoil, etc. But we will use Redux for this project.

Redux used to be very complicated and also we had a lot of packages with us. So we shifted towards Redux Tookit to solve our matters from the Redux.

Redux tookit is also known as "RTK".

Redux store is very bug JS Object with all the values and it is kept in a central place. Any component can access this store here.

We have slices in our Redux store so that the store does not become to much heavy in the context.

Logical Partitions are slices inside a Redux Store.

When we click on Add button, it will dispatch an action to the store and the store will update the state and the component will re-render.

When an action is dispatched, it will call a function and this will modify the cart. This function is called as Reducer.

We use a selector to dispatch the value from the store to the component. Selector will modify our read data. This phenomenon is called as subscribing to the store.

Only two libraries are installed: react-redux and @reduxjs/toolkit, and this will make our app use redux easily.

We will provide our store to our application using the Provider. Provider will be imported from the react-redux package. Provider will take the store as an attribute here and will do the work as required by the Provider of providing the store values to our application.

We also need to create the cart slice and for that we need to add some properties here into the cart{name, initialState:{
    items:[]
}, reducers}.

In reducers, we have an action type and a function linked to it so that it dispatch an change in cart when ever that action occurs.

A typical function looks like: 

addItem :(state, action)=>{
    state.items.push(action.payload)
}

Subscribing to a store is done by using the selector:
const cartItems = useSelector(state=>state.cart.items) and we need to access only this section of the cart.

Now here we can get all the cart items here.

On click of a button, we need to dispatch an action so that it will dispatch the action for the click of a particular type of button.

Dispatching an action is doen by using the hook called as useDispatch. Now we know it also has a value inside it that will be passed out, so that is also called as the payload that we are going to pass inside it. This will be added, removed from the cart on respective call of the button.

This is what we call the action.payload that we are passing.

When passing a function on event, this can be done by using {function} or {()=> function()}. The latter will create a new function every time it is called. The former will only take a reference and then call the function by taking reference from there.

We can again get the items in the cart by subscribing it to the redux store and then we can get the items from the store.

When using the redux store, do subscribe to the right section of the store.

If we are taking a store and then returning that store only, and then taking out the items from it, it will be an efficient way of coding here.

In redux store, we have a single reducer and in slice, we have multiple reducers in our existence.

In the cartSlice, we are actually returning a reducer from out there and reducer itself is a collection of various reducers out there.

In older versions of redux, it was not allowed to mutate the state out there. eg: now we can use the system of state.items.push or state.items.pop by using the impure function to modify the state of the store.

Earlier we used to make a new state out of it by making a copy of the state and then we used to change that new state and return it.

Immer takes care of all the state changes and what all things are done by the redux. Immer itself allows us to work with immutable state in more convenient ways. Also in new verison of redux, we don't need anything to return here.

We are not actually changing the state or mutating the state, it is just that we are adding a reference to it.

If i make the state as [], it will create a new reference to the state and our state will not change originally so we don't use this concept here, so we make the state's length as 0.

Redux creates a proxy object in behind the scenes and not the simple array, so to console it, we need console.log(current(state)).

Redux toolkit saysy either we should return the new state or mutate the state. So if we don't want to use the state.cart.length = 0, so we can just return the [] by using return {items:[]}.

Redux Dev Tools: Tools used to debug the application if we are using redux with us.

We have a trace that it shows where the data is being called away.

I can jump onto any state and it will not even show any error. We can even simulate the state behaviour here. It is very helpful for us to do debugging behaviour here.

In older versions of react, we used to use redux thunk or middlewares, but now we use to use the RTK Query.
