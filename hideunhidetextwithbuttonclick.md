# Hide and Unhide Text With a Button CLick and also Change The Button Label as Well As the Condition 
* HideUnhide.js Code will be like below 
```js
import { useState } from "react"

function HideUnhide(){
    const [flag,setFlag]=useState(false)
    
    // if(flag){
    //     var buttonflag  = "Hide The Data"
    //     var data        = "Hello How Are You" 
    // }
    // else{
    //     var buttonflag  = "Unhide The Data"
    //     var data        = null
    // }
    // return (
    //     <center  
    //         {data}
    //         <button onClick={()=>setFlag(!flag)}>{buttonflag}</button>
    //     </center>
    // )

    return (
        <center>
            {flag ? "Hello How Are You " :null}
            <button onClick={()=>setFlag(!flag)}>{flag? "Hide the Data": "Unfide the Data"}</button>
        </center>
    )
}
export default HideUnhide
```
