## Ternary Operator 
![](https://github.com/itzsnehasis/Reactjs/blob/main/Gallery/9PWZprmaRn.gif)

* Setting up the component
```js
import {useState} from 'react'

function Ternary() {
    const [user,setUser] = useState(2)
    return(
        <center>
            {
                user==1?<h1>User 1</h1> : user==2?<h1>User 2</h1> : <h1>Guest</h1>
            }
        </center>
    )
}

export default Ternary;
```
