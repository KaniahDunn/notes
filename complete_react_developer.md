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
    - 

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