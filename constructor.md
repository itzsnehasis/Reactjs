## Why we need constructor ?
constructor use for basically calling something even before render ...

## How to create a Constructor 
```js
//in Aclasscmp.js

import React from 'react'
class Aclasscmp extends React.Component{
    constructor(){
        super()
        console.log("I am Constructor")
    }
    render(){
        console.log("I am From Render")
        return (
            <center>
                <div>Hello I am Class Component</div>   
            </center>
        )
    }
}

export default Aclasscmp
```
* `super()` is for calling parent constructor `Component`
