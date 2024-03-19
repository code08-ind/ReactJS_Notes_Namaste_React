# Finding The Path

useEffect will be called after every render of the component. Without Dependency Array, useEffect will be rendered every time the component is rendered. With Dependency Array, useEffect will be rendered only when the dependency is changed.

If the dependency array is empty, it is rendered only once the page is loaded and called only on initial render and just once.

If we put a dependeny inside the array, it will only rendered again if the dependency is changed and called everytime when the dependency changes.

Don't make state variables outside the components. Don't use the state variables inside the if statements. Never create state variables inside the for loop and don't create state variables inside a normal function.

react-router-dom will be used here for the routing itself.

We have a createBrowserRouter that will create the browser router and we have a RouterProvider that basically provides the routing configuration to our application. We have certain components inside the createBrowserRouter that are element, path and errorElement.

react-router-dom also provides us with useRouteError hook that helps us to get more information about the error and show a specific error to the user.

Outlet will be filled according to the path and the component will be shown out there. Outlet comes from react-router-dom.

Two Types Of Routing in web apps:
1. Client Side Routing: The browser has codes for those components only and this only loads the component out there. This is a single page application here and implementing client side routing.
2. Server Side Routing: We make a server call, and the data comes from the server side.

We should speak while we code inside interviews.

Graphql is used to only fetch the data that is required for us. Link tag also uses a tag inside it only as it only runs on the frontend or client side itself.

We can also use useRouteError hook to make the route go to the Error Page.
