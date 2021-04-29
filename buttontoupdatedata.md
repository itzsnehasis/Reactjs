# Making a button to update data by click 
1.The code in Button.js
```js
import react, { useState } from 'react'
function Button(){
    // declearing a variable named user and initailizig "swarna" at first sate 
    const [user, setData]=useState("swarna")
    function updateData() {
        // declearing what to set after button click
        setData("Snehasis")
    }
    return(
        <center>
            <h1>Hello {user}</h1>
            <button onClick={updateData}> click me ! </button>
            {/* direct alert function with arrow function */}
            {/* <button onClick={()=>alert("Hello")}> click me ! </button> */}
        </center>
        
    )
}

export default Button;
```
