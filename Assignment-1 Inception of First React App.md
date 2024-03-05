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
