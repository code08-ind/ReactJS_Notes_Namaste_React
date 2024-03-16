1. **What is JSX?**
   JSX stands for JavaScript XML. It is a syntax extension for JavaScript which allows developers to write HTML-like code within JavaScript. JSX makes it easier to write and visualize the structure of UI components, especially in React applications. JSX gets compiled into regular JavaScript functions by tools like Babel before it gets executed in the browser.

2. **Superpowers of JSX**
   - **Combining Markup with JavaScript**: JSX allows developers to write HTML-like syntax directly within JavaScript code, enabling them to easily combine UI markup with JavaScript logic.
   - **Component-based Architecture**: JSX facilitates the creation of reusable components, promoting a modular and structured approach to building UIs.
   - **Efficiency and Readability**: JSX code tends to be more concise and readable compared to traditional JavaScript DOM manipulation, making it easier for developers to understand and maintain their code.
   - **Static Type Checking**: JSX can be used with TypeScript or Flow, enabling static type checking for better code quality and fewer runtime errors.
   - **Inline Styling**: JSX supports inline styling, allowing developers to define styles directly within component code using JavaScript objects.
   - **Dynamic Content**: JSX supports dynamic content rendering, allowing developers to easily incorporate JavaScript expressions and variables within JSX code.

3. **Role of type attribute in script tag? What options can I use there?**
   The `type` attribute in the `<script>` tag specifies the type of script being used. The most common values for the `type` attribute are:
   - `text/javascript`: This is the default value if the attribute is not specified. It indicates that the content of the script element is JavaScript code.
   - `module`: Indicates that the script is a module script, allowing the use of JavaScript modules.
   - `text/jsx`: Used when including JSX code directly in HTML files. This tells the browser to interpret the content as JSX.

4. **{TitleComponent} vs {<TitleComponent/>} vs {<TitleComponent></TitleComponent>} in JSX**
   - `{TitleComponent}`: This syntax is used to render the `TitleComponent` as a child element. It assumes that `TitleComponent` is a variable containing a React component, and it will be rendered as is.
   - `{<TitleComponent/>}`: This syntax is used to render the `TitleComponent` component directly. It's a self-closing tag indicating that `TitleComponent` should be instantiated as a React component and rendered at that point.
   - `{<TitleComponent></TitleComponent>}`: This syntax is similar to the previous one, explicitly opening and closing the `TitleComponent` element. While functionally similar to `{<TitleComponent/>}`, it provides a more explicit delineation of the component's start and end.
