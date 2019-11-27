### ./reducers
#### index.js
```javascript
import {combineReducers} from 'redux';
import ___Reducer from './___'
import ___Reducer from './___';

const allReducers = combineReducers({
    ___: ___Reducer,
    ___: ___Reducer
})

export default allReducers;
```

#### ___Reducer.js
```javascript
const ___Reducer = (state = initState, action) => {
    switch(action.type) {
        case '': {
            return satate;
        }
        case '': {}
        default: {}
    }
}
export default ___Reducer
```

### ./actions
#### index.js
```javascript
export const increment = () {
    return {
        type: 'INC',
        payload: null
    }
}
```


### ./
#### index.js
```javascript
import { createStore, applyMiddleware, compose } from 'redux';
import allReducers from './store/reducers';
import { Provider } from 'react-redux';
import reduxThunk from 'redux-thunk'


const store = createStore(
  allReducers, 
  compose(
    applyMiddleware(reduxThunk),
    window.__REDUX_DEVTOOLS_EXTENSION__ && window.__REDUX_DEVTOOLS_EXTENSION__(), 
  )
);

ReactDOM.render(
    <Provider store = {store}>
        <App />
    </Provider>,
    document.getElementById('root')
);
serviceWorker.unregister();
```

#### App.js
```javascript
import { useSelector, useDispatch } from 'react-redux';

function ___() {
    const val = useSelector(state => state.val);
    const dispatch = useDispatch();

    // () => {dispatch({type: '...', payload: '...'})}
}
```
