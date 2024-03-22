1. **Microservice:**
   A microservice is an architectural style where an application is built as a collection of loosely coupled, independently deployable services. Each service is focused on performing a single business function and communicates with other services through well-defined APIs, typically over HTTP. Microservices promote modularity, scalability, and flexibility in software development.

2. **Monolith architecture:**
   Monolith architecture refers to a traditional approach where an entire application is built as a single, self-contained unit. In a monolithic architecture, all components of the application, including the user interface, business logic, and data access layers, are tightly integrated and deployed as a single unit.

3. **Difference between Monolith and Microservice:**
   - Monolith: Single, self-contained application unit. Tightly integrated components. Deployed as a single unit.
   - Microservice: Collection of loosely coupled, independently deployable services. Each service focuses on a single business function. Communicates with other services through APIs. Deployed independently.

4. **useEffect Hook:**
   `useEffect` is a React Hook used for handling side effects in functional components. It allows you to perform tasks such as data fetching, subscriptions, or manually changing the DOM in response to component lifecycle events, such as mounting, updating, and unmounting.

5. **Optional Chaining:**
   Optional chaining is a feature introduced in JavaScript (as part of ECMAScript 2020) that allows you to access properties of an object without the need to explicitly check if each level of the chain is not null or undefined. It is denoted by the question mark (`?.`) and short-circuits the evaluation if any part of the chain is null or undefined.

6. **Shimmer UI:**
   Shimmer UI is a design pattern used to indicate to the user that content is loading or that an area of the interface is currently inactive. It typically involves displaying animated placeholder elements that mimic the structure of the expected content until the actual content is loaded.

7. **Difference between JS expression and JS statement:**
   - Expression: Produces a value. Can be a variable, literal value, function call, or combination of these with operators. Examples include `2 + 2`, `myFunction()`, `true ? 'yes' : 'no'`.
   - Statement: Performs an action. May not necessarily produce a value. Examples include variable assignments (`let x = 5;`), control flow statements (`if`, `for`, `while`), and function declarations.

8. **Conditional Rendering:**
   Conditional rendering refers to the practice of rendering different parts of a user interface based on certain conditions. In React, this is often achieved using JSX and JavaScript logical operators. Example:

   ```jsx
   function App() {
     const isLoggedIn = true;
     
     return (
       <div>
         {isLoggedIn ? <UserDashboard /> : <Login />}
       </div>
     );
   }
   ```

   In this example, if the user is logged in (`isLoggedIn` is `true`), the `UserDashboard` component is rendered; otherwise, the `Login` component is rendered.

9. **CORS (Cross-Origin Resource Sharing):**
   CORS is a security feature implemented by web browsers that controls access to resources located on a different origin (domain) from the one that served the web page. It is used to protect users by preventing malicious scripts from accessing resources they should not have access to.

10. **async and await:**
    `async` and `await` are keywords used in asynchronous JavaScript programming to simplify the syntax of working with promises. 
    - `async` keyword is used to define a function as asynchronous, allowing it to use the `await` keyword.
    - `await` keyword is used to pause the execution of an async function until a Promise is settled, and to resume execution of the async function after the Promise is fulfilled, returning the resolved value.

11. **`const json = await data.json();`:**
    This line of code is an example of using the `await` keyword to asynchronously fetch and parse JSON data. It is typically used in conjunction with the Fetch API in JavaScript. `data.json()` returns a Promise that resolves to the JSON representation of the response body, and `await` waits for that Promise to resolve, assigning the parsed JSON data to the variable `json`.
