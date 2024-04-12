# Time for Test

Different Types Of Testing A Developer Can Do:

1. Manual Testing: We are manually testing different components.
2. Developer can do testing with certain types:

    - Unit Testing: Testing individual components.
    - Integration Testing: Testing multiple components together.
    - End-to-End Testing: Testing the whole application.

Unit Testing: We test our components individually or in isolation.
Integration Testing: We test multiple components together.
End-to-End Testing: We test the whole application.

Testing is a part of writing code and it is a part of developers lives.

We will be using React Testing Library To Write Test Cases In Our Application. 

All the testing libraries are based on DOM testing libraries. When we use create-react-app, we have prebuild react testing library.

React Testing Library is having Jest: Jest is nowadays used as Delightful Js testing Framework.

Steps:

1. Install React Testing Library: `npm install @testing-library/react.
2. Install Jest: `npm install -D jest`.
3. We are using Jest using Babel. So let us install: npm i -D babel-jest @babel/core @babel/preset-env.
4. Configure Babel.
5. Babel is configured in our application using babel.config.js.

Parcel conlicts with babel, so we need to change the parcel configurations for babel.

We want our testing library jest to work properly, so we need to change the parcel.rc file here in our system. This code can be found on parcel documentation.

We need to configure babel also by using the babel.config.js file.

npm run test, it is the command that is used to run tests in our file.

Now we will do jest configuration: npx jest --init.

It will ask us certain questions. jsdom is the env similar to our browser.

Now we have to install the jsdom library separately here. For jest to work properly, we have to install jest-environment-jsdom separately.

Our tests are stored in a directory named: __tests__. Now jest will try to match the files for tests in this folder with the extensions of js or ts files.

Naming convention of the files will be: Headers.test/spec.js/ts 

__ = dunder, so we also call tests as dunder tests.

We write the test cases by using the concept of:

It takes description and a function. We can write our test cases inside this function. And inside it takes the function which we want to test out here.

test("Sum will calculate sum of two functions", ()=>{
    const sum = sum(3,4);

    Assertion is done here
    expect(sum).toBe(7);
});

If we are not expecting anything, it will always pass.

Now we will work with unit testing.

If we want to check if a component gets render on the jsdom, and we will use render method for that. 

By using screen method from redux toolkit, and we can get the thing by using getByRole here.

Now i want this heading component in my document or not.

JSX Will only work when we have @babel/preset-react with us. We will install it and with this it will work properly.

In babel.config.js, we will put this into our array, so we will insert a thing inside it to make the runtime automatic here with @babel/preset-react.

We Will Install the library jest-dom from react testing library. 

To check if a component loaded successfully in the dom, we will check using toBeInDocument here.

We can get the text by using .getByText(), we will find the text using text from the link.

We can even try for get by placeholder text here.

We can even by using .getByRole or .getAllByRole, we can get the role of the component even if we have multiple roles here and not give error here. It returns different Jsx components from virtual DOM.

We can also get the length of the components here and we can expect the length of input boxes to be expected as the length we expect out.

We can use describe block to define multiple test cases here and define them there.

We can also write name of test as it as well inside the describe block:

```javascript
describe("Header Component", ()=>{
    it("Header Component Renders Correctly", ()=>{
        render(<Header />);
        expect(screen.getByRole("heading")).toBeInTheDocument();
    });

    test("Header Component Contains Text", ()=>{
        render(<Header />);
        expect(screen.getByText("Header")).toBeInTheDocument();
    });
});

```

.toBeTruthy will tell about more about the values such as true or false. If we want to test a component that uses store, so we need to provide a store for it here.

If we are also testing the BrowserRouter, we need to include this as well in our components here inside our testing files.

If we want to find the button with a specific name, this can be done by using the screen.getByRole("button", {name:"Login"}).

We can also find the the cart items in the header by using the .getByText thing here.

We can also run a function on click function by using fireEvent.click(loginButton).

We can also load data by using props.

To test a component, we need to pass the mock data inside it. It will render the mock data and find any text inside it if it exists or not.


### Integration Testing

We can also create test cases for fetching the api as well. When it renders, it renders the code on jsdom and not the browser. Jsdom is similar to browser, but it does not match fully to the browser like features.

So to make fetch work, we need to fake the fetch function.

```javascript
global.fetch = jest.fn(()=>{
    return Promise.resolve({
        json: ()=>Promise.resolve(data);
    });
});
```

If we want to make test cases to run on hot reload, use: npm run jest --watch

So we should wrap our render method inside the act function. act function is await. act will take the async function inside it and then it will be having a callback function inside it and this will render the component here. Again we will render the Body component inside the BrowserRouter itself.

act function comes from react-dom/test-utils, this test case will be noted down as the async await function. act again takes the callback function and it will take the render method inside it.

If we get any error regarding the Link tag error, make the browserrouter to be outside Body we are using.

We can also get the screen.getByTestId. This will allow us to get the items in my input text box which has a property data-testid attribute.

Now we want to change the text box, so we will fireEvent .change event. We have a target here inside it which tells what we want to write inside it as a target element.

This is how we run different test cases in our system with different issues involved on our application.

We are having a function called beforeAll() which will run before everything here in the system. beforeEach() is run before running each test case.

Similarly we have afterAll and afterEach functions to run after each or after all.

If we are using the testing criteria over the header menu where we require the cart menu here, we can do this by using the keeping that component inside the Provider that will have the store inside it.

We can see more details about the coverage of the test cases by using the index.html in coverage folder and it will give us more details about it.
