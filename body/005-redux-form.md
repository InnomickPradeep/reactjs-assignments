### Objectives

After this exercise, you should be able to:

- Know about the reactredux and redux form and implementing  axios calling using react redux
- For axios need to be aware of Action ,Reducer and Api calling and Fetching the data


### Example
-React Redux is the official React binding for Redux. It lets your React components read data from a Redux store, and dispatch actions to the store to update data.

creating an example using props and state

import React from 'react' 
import ReactDOM from 'react-dom'

import { Provider } from 'react-redux'
import store from './store'

import App from './App'

const rootElement = document.getElementById('root')
ReactDOM.render(
  <Provider store={store}>
    <App />
  </Provider>,
  rootElement
)

## Action
export const deleteData = (url, props) => {
    return (dispatch) => {
        axios.delete(url)
        .then(response => {
            dispatch(deleteDataSuccess(response));
        })
        .catch(error => {
            //TODO: handle the error when implemented
        })
    }
}

## Reducer 
const reducer = (state = initialState, action) => {
    switch (action.type) {
        case actionTypes.GET_DATA_SUCCESS:
            return executeGetDataSuccess(state, action);
        case actionTypes.POST_DATA_SUCCESS:
            return executePostDataSuccess(state, action);
        case actionTypes.PUT_DATA_SUCCESS:
            return executePutDataSuccess(state, action);
        case actionTypes.DELETE_DATA_SUCCESS:
            return executeDeleteDataSuccess(state, action);
        default:
            return state;
    }
}
export default reducer;

### Exercise

1. create a Action ,Reducer file and call the Axios Api and need to fetch the data
2. Click the **Save** button to save your changes.
3. Run the Application
4. If your tests pass, you will able to see the Api call in Network in the developer console.