1. створити store

<!--
import { configureStore } from '@reduxjs/toolkit'

export const store = configureStore({
  reducer: {},
})
 -->

2. Обгорнути Провайдером компонент App
<!-- 
import { store } from './app/store'
import { Provider } from 'react-redux'

ReactDOM.render( <Provider store={store}> <App /> </Provider>,
document.getElementById('root') ) -->

3. Зробити редюсер
<!-- 
const counterReducer = createReducer(0, {
  increment: (state, action) => state + action.payload,
  decrement: (state, action) => state - action.payload,
})

console.log(counterReducer.getInitialState()) // 0 -->

4. Зв'язати редюсер і стор
<!--
export const store = configureStore({
  reducer: {
    contacts: phoneBookReducer,
  },
});
 -->

5. Створити action
<!-- import { createAction } from '@reduxjs/toolkit';

export const addContact = createAction('phoneBook/addContact'); -->
