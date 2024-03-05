Episode 1 Inception Of JavaScript

We can create an element in html by using javascript, this can be done by using the document.createElement("h1") and then appending it inside a different element in the document.

We can even include the cdn links of react.js and we can also include react here. Now browser can understand the react code.

CDN Links: These CDN Links will include all of the random shit

<script crossorigin src="https://unpkg.com/react@18/umd/react.development.js"></script>
<script crossorigin src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>

crossorigin: 

The crossorigin attribute in HTML's <script> tag sets the request mode to an HTTP CORS Request. It's used to load an external script into a domain from a third-party server or another domain. 

The crossorigin attribute sets the mode of the request to an HTTP CORS Request. Web pages often make requests to load resources on other servers. Here is where CORS comes in. A cross-origin request is a request for a resource (e.g. style sheets, iframes, images, fonts, or scripts) from another domain.

This attribute is used to protect sensitive information from the third party when fetching out the results. It also defines how the element handles cross-origin requests. 

Cross-origin requests are requests for a resource from another domain. These resources may include style sheets, iframes, images, fonts, or scripts. The crossorigin attribute is valid on the following elements: <audio>, <img>, <link>, <script>, <video>. 

Now we have the React code inside our repository and we can do anything about here in React. We also have some Secret Internals: Don't use otherwise you will be fired. Hahaha !!!

Second cdn is basically combining off to provide the tools for the React DOM.

const heading = React.createElement("h1",{class:"head", id:"hello"},"Hello World"). We also need a root that will be created by ReactDom.createRoot(document.getElementById("root")). Then we have to use render method, root.render(heading). We can also give attributes here using it.

This is the real JavaScript. Most expensive operation in DOM is when we change some nodes or we either put some updates in DOM.

React will go to manipulating dom using React.

We will include multiple children inside the child nesting simply because. We add an object and while it is rendering, that itself converts that object into an HTML DOM. We can also add more than one child here, so we can just use the array of children. We need a key to for each unique child.

React can be written using the javascript as well in place of the jsx. Order of files matter as this will allow us to make use of the libraries and for it we need the actual javascript file need to be used later after the use of library files.

If there is anything inside the div#root, anmd if we add something inside the div#root externally, then that will replace the text that will be already be there inside the div#root.

React is a Library as everything is created on only a single page itself.

Extra Important Questions Of Assignment-1:

- **Emmet:** Emmet is a toolkit for web developers that vastly improves HTML and CSS workflow. It allows for the quick generation of HTML and CSS code using abbreviations. For example, typing `ul>li*5` and then expanding it with Emmet would generate an unordered list with five list items.

- **Difference between a Library and Framework:**
  - **Library:** A library is a collection of reusable code that can be imported and used in various projects. It provides specific functionalities that developers can use as needed. Libraries do not enforce a particular structure or architecture on the project.
  - **Framework:** A framework, on the other hand, provides a more comprehensive structure for building applications. It often dictates the architecture of the application and requires developers to adhere to its conventions. Frameworks typically provide a set of tools, libraries, and guidelines to streamline development.

- **CDN (Content Delivery Network):** A CDN is a network of distributed servers that deliver web content to users based on their geographic locations. It helps to reduce latency and improve website performance by serving content from servers that are closer to the user. CDNs are used to deliver static content such as images, scripts, stylesheets, and other media files.

- **Why is React known as React?:** React is called React because of its main concept, which is to "react" to state changes. It efficiently updates and renders the user interface in response to changes in application state, leading to a more dynamic and responsive web application.

- **crossorigin in script tag:** The `crossorigin` attribute in a script tag is used to specify how the browser should handle requests when loading scripts from a different origin (i.e., a different domain, protocol, or port). It is typically used when loading scripts from a CDN or a different domain to ensure that CORS (Cross-Origin Resource Sharing) policies are followed.

- **Difference between React and ReactDOM:**
  - **React:** React is the core library for building user interfaces in React applications. It provides the fundamental mechanisms for defining components, managing component state, and rendering UI elements.
  - **ReactDOM:** ReactDOM is a package that provides DOM-specific methods for React. It is used to render React components into the DOM (Document Object Model) and manage interactions between React components and the DOM.

- **Difference between react.development.js and react.production.js files via CDN:**
  - **react.development.js:** This file contains the development version of the React library. It includes additional warnings and debugging information to aid developers during development and debugging stages.
  - **react.production.js:** This file contains the production version of the React library. It is optimized for performance and does not include any debugging information or additional warnings. It is intended for use in production environments to reduce file size and improve runtime performance.

- **async and defer:** Both attributes are used in the script tag to control the loading and execution of external scripts.
  - **async:** The `async` attribute tells the browser to load the script asynchronously while continuing to parse the HTML document. The script will be executed as soon as it is downloaded, which may happen concurrently with the parsing of the HTML document. This is useful for scripts that do not depend on the HTML document's structure.
  - **defer:** The `defer` attribute tells the browser to defer the execution of the script until after the HTML document has been fully parsed and displayed. Multiple scripts with the `defer` attribute will be executed in the order they appear in the document. This is useful for scripts that need to access and modify the DOM.
