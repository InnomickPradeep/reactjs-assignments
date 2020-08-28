### Objectives

After this exercise, you should be able to know:

- What are the life cylce methods ?
- Why we use life cycle methods in react and their advantages ?
- how each life cycle method works and their importance

### Example

-React components have several special methods that provide opportunities to perform actions at specific points in the lifecycle of a component. These are called lifecycle methods, or lifecycle hooks, and allow you to catch components at certain points in time.
-Use different life cycle methods in a class component and try to console them and verify in browser.


```react
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
  }
  componentWillMount() {
      console.log("componentWillMount")
    // change code below this line

    // change code above this line
  }
  componentDidMount(){
    console.log("componentDidMount")
  }

  // should use remaining life cycle methods like above 
  render() {
    return <div />
  }
};

```



### Exercise

1. create a file of class component and implement each life cycle method independently 
2. use different life cycle methods and console them and verify in in the browser console to verify  the life cycles 
2. Click the **Save** button to save your changes.
3. Run the Application
4. If your tests pass, you will see your application in the browser