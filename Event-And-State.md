## Let we have a input box we can input text there and how the texts can be printed anywhere without reloading the page as soon as you type
![](https://github.com/itzsnehasis/Reactjs/blob/main/Gallery/sMC4l2utHu.gif)

1. lets make a component named Input.js which will contain a input box for us 
```js
function Input() {
    const [data,setData]=useState();
    return(
        <center>
            <h1>{data}</h1>
            <input type="text"/>
        </center>
    );
}

export default Input;
```
2. Now if we import and use this Component in Index.js we will see that input box in our home page 
```js
import ReactDOM from 'react-dom';
import './index.css';
import Input from './Input';
import reportWebVitals from './reportWebVitals';

ReactDOM.render(
  <React.StrictMode>
    <Input/>
  </React.StrictMode>,
  document.getElementById('root')
);

reportWebVitals();
```
3. Lets go back to Input.js and lets define the event by editing line 9 to `<input type="text" onChange={getData}/>`
4. The Complete Index.js Will be like This 
```js
import { useState } from "react";


/*function Input() {
    const [data,setData]=useState();    
    function getData(val) {
        setData(val.target.value);        
    }
    return (
        <center>
            <h1>{data}</h1>
            <br></br>
            <input type="text" onChange={getData}/>
        </center>
    )
}*/
 

function Input() {
    const [data,setData]=useState();
    return(
        <center>
            <h1>{data}</h1>
            <input type="text" onChange={event=>setData(event.target.value)}/>
        </center>
    );
}

export default Input;
```
