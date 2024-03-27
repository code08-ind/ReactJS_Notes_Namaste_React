1. **How do you create Nested Routes in react-router-dom configuration?**
   
   Nested routes in `react-router-dom` can be created by nesting `<Route>` components within each other. For example:

   ```jsx
   import { BrowserRouter as Router, Route, Switch } from 'react-router-dom';

   function App() {
     return (
       <Router>
         <Switch>
           <Route path="/parent" component={ParentComponent}>
             <Route path="/parent/child" component={ChildComponent} />
           </Route>
         </Switch>
       </Router>
     );
   }
   ```

2. **Read about createHashRouter, createMemoryRouter from React Router docs.**

   - `createHashRouter`: It creates a router that uses the hash portion of the URL for routing. Useful for applications that need to support older browsers that don't handle HTML5 History API well.
   - `createMemoryRouter`: It creates a router that doesn't use the browser's URL but instead keeps the location in memory. Useful for server-side rendering or testing.

3. **What is the order of lifecycle method calls in Class-Based Components?**

   The order of lifecycle method calls in Class-Based Components is as follows:
   
   - `constructor`
   - `componentWillMount` (deprecated)
   - `render`
   - `componentDidMount`
   - `componentWillReceiveProps` (deprecated)
   - `shouldComponentUpdate`
   - `componentWillUpdate` (deprecated)
   - `render`
   - `componentDidUpdate`
   - `componentWillUnmount`

4. **Why do we use `componentDidMount`?**

   `componentDidMount` is used to perform actions after the component has been rendered to the DOM. It is commonly used to fetch data from an API, set up subscriptions, or perform any DOM operations necessary for the component.

5. **Why do we use `componentWillUnmount`? Show with example.**

   `componentWillUnmount` is used to perform cleanup actions before a component is removed from the DOM. For example, you might use it to unsubscribe from event listeners or clear timers to prevent memory leaks. Here's an example:

   ```jsx
   class Timer extends React.Component {
     constructor(props) {
       super(props);
       this.state = { time: 0 };
     }

     componentDidMount() {
       this.timerID = setInterval(
         () => this.tick(),
         1000
       );
     }

     componentWillUnmount() {
       clearInterval(this.timerID);
     }

     tick() {
       this.setState({
         time: this.state.time + 1
       });
     }

     render() {
       return (
         <div>
           Time: {this.state.time}
         </div>
       );
     }
   }
   ```

6. **Why do we use `super(props)` in the constructor?**

   We use `super(props)` in the constructor to call the constructor of the parent class (React.Component) and pass props to it. This is necessary because when defining a constructor in a subclass, we need to explicitly call `super()` to ensure that the parent constructor is properly initialized.

7. **Why can't we have the callback function of useEffect async?**

   The callback function passed to `useEffect` cannot be async because `useEffect` expects either a cleanup function or nothing to be returned synchronously. An async function always returns a Promise, which is not suitable for this purpose. Instead, you can create a separate async function inside the `useEffect` callback and call it within the callback.
