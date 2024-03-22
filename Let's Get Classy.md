# Let's Get Classy

We will be discussing about the Class Based Components. Class components will have a render method, they will return some piece of jsx.

Constructor inside the class based components will recieve the props by using super(props) because it is the only place to set up our initial state and bind event handlers before the React component mounts.

Any variable can be used from props using the this.props.name and will allow us to use props anywhere in the class.

Inside a class based component, it is best way to create state variables inside the class variables. States can be accessed using the this.state etc.

Never update state variables directly. this.setState() method should be used to update the state variables and pass the object will contain the updated value of all the variables. We can pass multiple states inside a particular object by passing the data.

When we pass a particular data out there, we will only update that particular state and the rest of the states will remain the same.

React Lifecycle Methods in class Based Components.

When the component is mounted, jsx is rendered. Once class is loaded, constructor is called and rendered is used then.

ComponentDidMount is called when the component is fully loaded or mounted in the system. ComponentDidMount is used for making the API calls.

First parent constructor is called, parent render, child constructor, child render is called, child component is mounted, parent component is mounted.

First all the child component constructor is called, render is called and after that first child component is mounted, then second child component is mounted and finally parent component is mounted. Once react updates the DOM, then react will mount the component.

Render phase has constructor, render method. In commit phase we actually update the DOM. 

First Render phase of both the components is completed and then commit phase of both the components is completed.

DOM Manipulation is the most costly process when we load the component here.

DOM is updated in batching here itself before the components are mounted inside the system.

We can make componentDidMount as async here and call the data by fetching the data from the api call and await the data here.

Lifecycle is done in the form of:

Mounting

Constructor(dummy data)
Render(dummy data)
    <HTML (dummy data)>
ComponentDidMount
    <Api calls>
    <this.setState> -> state variables is updated

UPDATE

    render(API data)

    <HTML (new API data)>

    componentDidUpdate(API data)

componentDidUnmount()

Never compare Lifecyle events with Functional components hooks. If we want to do multiple things out there, we can use the more than one useEffect hooks for different variables.

We unmount the component when ever we go to other component on that page itself, as we are having componentDidMount which will be called everytime when the component is mounted here. If we have to clear a data resource, we can use componentWillUnmount and use it to clear the code here.

If we have return inside useEffect, it will be called when we switch from that component or skipping the page and this acts a unmounting phase here.

```
return ()=>{
    clearInterbal(interval) 
}
```

Popular React Lifecycle Methods Used Are:

componentDidMount
componentWillUnmount
componentDidUpdate
shouldComponentUpdate
constructor and render.
