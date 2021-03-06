### Complete React Developer Notes

#### React Key Concepts 
- Impertative vs. Declarative 
    - Imperative: When the developer or designer directly changes componenets or aspects of an application in response on a users events
    - Declarative: Given a state on how any application should look and act and is then controlled by user action without having to manipulate the DOM everytime

- Components Architecture 
    - js function that recieve input or attributes/props that return HTML 
    - can be functional or class based 
    - easy to resuse and recycle 

- Directional Data Flow
    - data can only move down from state to different components in the application 

- NPX command is a way run a command of a package in the terminal without having to install it explicitly

- Babel vs. Webpack 
    - Babel helps build and compile code so that it works on all versions of different web browsers 
    - Webpack condensese JS files so that they can be read and used in the browser

### React Basics 

- Functional vs. Class Components 
    - Class compoments are the archaic way of writing React 
    - Functional components are the more preferred way 

- Life-cycle Methods 
    - ComponentDidMount: is used when the component is first rendered to the DOM 
 
- setState 
    - An asynchronous function call 
    - JS doesn't wait to for the rest of the code to be run before this call/function is done processing
    - For example when console logging the state below, you will see that the state isn't actually set right away after typing the first element when the onChange function is called 
    ```
    onChange={
            e => this.setState({ searchField: e.target.value }
            )
          }
    ```

    - To see state change as someone is typing in the search bar, a call back function can be used as shown below 

    ```
    onChange={
            e => this.setState(
              { searchField: e.target.value },
              () => console.log(this.state)
            )
          }
    ``` 

- Synthetic Events 


- Destructing : The ability to pull property off of an object and set them to `const` variables 

- Actual DOM vs. Virtul Dom 
    - Actual DOM that is presented in the browser 
    - Virtual DOM is a copy that a created by React to update when there are changes to the Data that is being rendered to the components in the Actual DOM. React with look at the changes made to the components and their data, make a copy and then compare that against the actual DOM and render that SPECIFIC change to the actual DOM rather than rendering an entire new actual DOM. 