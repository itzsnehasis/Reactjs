## Passing Function Through Props
![](https://github.com/itzsnehasis/Reactjs/blob/main/Gallery/eRhNHrL3go.gif)



1. Setting the component which will send the function 
```js
//in Sender.js

import Reciver from './Reciver'
function Sender() {
    function getData() {
        alert("I am From Sender")
    }
    return(
        <div>
            <Reciver data={getData}/>
        </div>
    )
}

export default Sender
```
2. Setting up the component which will use the function of sender component
```js
//in Reciver.js

function Reciver(props) {
    return (
        <center>
            <div>
                <button onClick={props.data}>Click Me</button>
            </div>
        </center>
    )
}

export default Reciver
```
