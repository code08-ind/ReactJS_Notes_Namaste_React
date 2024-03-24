# Let's Optimize Our App

We should modularize our app so that our code becomes maintainable, testable and work wonderfully here.

Creating a custom hook will make the code look amazing and work beautifully.

We can basically make use of the custom hooks here and make our functions run accordingly here.

It is not mandatory to use before the custom hook name.

Chunking 
Code Splitting
Dynamic Bundling

We want a bundle should have enough code for a feature that is the one part of the component inside an application. We should build out various bundles for various of the components in an application. 

We should build up logical bundling here.

We will include our component by using lazy loading because we don't want it to load to automatically. We want it to load only when it is required and it is also called on-demand loading.

Lazy loading can be used by using lazy() from React.
const Grocery = lazy(() => import('./Grocery'));

When we use lazy loading, we will make a different bundle for it for that component which will be loaded up on demand. The code tried to load the component but as it was lazy loading, so React suspended the call to load the component.

We have a component called as Suspense and add a fallback to it if a component is not there with us for the time being and it will display that message to the user when a function is performed here on the system.

Lazy loading is also called as Dynamic Import and to import when and where it is required up here.

Start From 01:00:00 Mins.
