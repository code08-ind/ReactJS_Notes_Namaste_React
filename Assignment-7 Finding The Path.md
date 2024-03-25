1. **Adding Images to an App:**
   There are several ways to add images to your app. Here are a few common methods:

   a. **Using `<img>` tag in HTML:**
   ```html
   <img src="path/to/your/image.jpg" alt="Description of the image">
   ```

   b. **Importing images in JavaScript (for frameworks like React):**
   ```jsx
   import React from 'react';
   import imageSrc from './path/to/your/image.jpg';

   function App() {
     return <img src={imageSrc} alt="Description of the image" />;
   }

   export default App;
   ```

   c. **Using CSS background image:**
   ```css
   .image-container {
     background-image: url('path/to/your/image.jpg');
   }
   ```

   d. **Using inline styles in JSX (for frameworks like React):**
   ```jsx
   import React from 'react';

   function App() {
     return (
       <div style={{ backgroundImage: `url(path/to/your/image.jpg)` }}>
         {/* Other components */}
       </div>
     );
   }

   export default App;
   ```

2. **console.log(useState()):**
   If you do `console.log(useState())`, it will log an array with two elements: the current state value and a function that allows you to update that state. This is because `useState()` returns an array with two elements.

3. **Behavior of useEffect without a dependency array:**
   If you don't add a dependency array to `useEffect`, it will run on every render cycle. This can lead to performance issues, unnecessary re-renders, and potentially infinite loops if the effect updates the state and causes a re-render.

4. **SPA (Single Page Application):**
   SPA stands for Single Page Application. It's a web application or website that interacts with the user by dynamically rewriting the current page rather than loading entire new pages from the server. SPAs often use AJAX and HTML5 to create fluid and responsive user experiences.

5. **Client Side Routing vs Server Side Routing:**
   - **Client-Side Routing:** In client-side routing, navigation and rendering of different views are handled by JavaScript running on the client's browser. When a user navigates within the application, instead of requesting new pages from the server, the router manipulates the browser's history and loads the appropriate components or views dynamically. It provides a faster and more seamless user experience since only the necessary components are fetched from the server.

   - **Server-Side Routing:** In server-side routing, navigation triggers requests to the server for different pages. Each navigation action leads to a full page reload as the server sends back the HTML for the requested page. This traditional approach can be less responsive compared to client-side routing since it involves fetching entire new pages from the server.

   The key difference lies in where the routing logic is executed: on the client-side (in the browser) for client-side routing, and on the server-side for server-side routing.
