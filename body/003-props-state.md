### Objectives

After this exercise, you should be able to:

- Know about the Jsx ,Props and state


### Example
-React uses a syntax extension of JavaScript called JSX that allows you to write HTML directly within JavaScript

creating an example using props and state

class StatefulComponent extends React.Component {
  constructor(props) {
    super(props);

    // initialize state here

  }
  render() {
    return (
      <div>
        <h1>{this.state.name}</h1>
      </div>
    );
  }
};

### Exercise

1. create a file of class component and implement state and props in it
2. Click the **Save** button to save your changes.
3. Run the Application
4. If your tests pass, you will see your application in the browser