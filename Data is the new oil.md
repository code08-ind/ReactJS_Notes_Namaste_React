# Data is the new oil

Higher order components: It is a function that takes a component and returns a component.

Higher order component is exported from the original file system and then it is imported into other file and now we get a variable defined out which takes takes the original component and returns a new component.

Higher Order Components Are Pure Functions.

Every React application has two layers: UI Layer and Data Layer inside it and UI Layer is powered by Data Layer.

We can build our own collapsible component by using the setItems(!items). and show items only when it is true.

React Deve tools extension will have two Layers: UI Layer and Data Layer where we can see the Props etc.

We also have Profiler section in our console, where it will record or profile all the things or activities we did here. This will record where we went, routes we used and things we did here and will show that components that are effected by the different components and we will also have a flamegraph here.

We can also lift up the state of the components here to the parent itself.

Controlled Components: We can control the state of the component by using the state of the parent component and by passing the props here.

Uncontrolled Components: We cannot control the state of the component from parent of the state of a child component.

We can open one collapsed component and Open the Other one by passing the state from the parent to the child component here. This will open one collapsed component and close the other one and a component can be passed too inside it easily here.

We should avoid Prop Drilling and to drill data to different levels.

React Context drilling should be used to have a global data and then pass that data to pass it to different components.

We have a hook called as useContext to use the context into our system. This can be used to get the context anywhere into our system here.

If we don't want a useContext hook, we can access the context using the <UserContext.<var_name>>

Inside it we have a callback function which calls the data here.

We can pass a value inside a component by using the <UserContext.Provider value={}> and in this way, we can pass the data inside the component to pass a value inside the component.

If we will pass only one component inside the <UserContext.Provider value={}>, we will only be able to see the context variable inside this variable.

We can use nested <UserContext.Provider value={}> and it will have a different value and the inner <UserContext.Provider value={}> will have a different value.

If we want to set the user data, we can also pass the setUserName into our application similarly by using the <UserContext.Provider value={{loggedInUser:userName, setUserName}}>

Important question here is that what is the difference between redux library and context api here.

We can build any large application using context. But redux is used nowadays to manage the state of the application.

Keep you data layer strong and automatically the UI Layer will remain strong.
