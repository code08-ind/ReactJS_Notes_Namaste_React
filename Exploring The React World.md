# Exploring the World

There are two API Approaches:
1. Loads Page -> API Called -> Render The Page.
2. Loads Page -> Render The Page -> API Called -> Re-Render The Page.
   
We will use the Second Approach. This gives us a better user experience.

React has some of the fastest Render Cycles.

useEffect will basically take the callback method as one argument and second argument uses the dependency array inside it. callback method will be called after the component is rendered. First the Body is rendered and then the callback method is rendered.

Browsers block us from calling api from one origin to another origin. We can allow CORS By using the Allow CORS: Access control allow cors.

We can see the API from the backend by going inside the network tab and find the api from there and call from there. Optional Chaining is a good way to write the code here itself. 

Here we will be using the Shimmer UI to load the fake pages until the original data is loaded up here. This is used inside the conditional rendering here which is used when we just show the data when the data is rendered when the data is being loading and we want to give a good user experience with beautiful user interface.

Normal JS Variables don't work here and local state variables come into consideration and special functions called hooks use to update the variables here in JSX to make the statement as Dynamic.

If an element is changed inside the Component, the whole component is re-rendered. This is the reason why we use the useEffect to make the component re-rendered only when the data is changed. When a state is changed, React is calling the component again after it gets rendered again.

Reconciliation Concept makes the React fast by rendering the components run fast.

Once we use the search functionality, we can use this by using the filtering the code and also once we have filtered the data, so again we need a copy here itself by re-changing the data by making a copy of the res.data and displaying it again once we have filtered the data.
