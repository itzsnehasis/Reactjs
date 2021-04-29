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
* Here We Can See Constructor is calling before rendering 
![](https://github.com/itzsnehasis/Reactjs/blob/main/Gallery/H1MMi03Fd9.gif)

## We can Apply this to define state before rendnering HTML Page

```js
import React from 'react'
class Aclasscmp extends React.Component{
    constructor(){
        super()
        this.state={
            data:"component"
        }
        // console.log("I am Constructor")
    }
    render(){
        // console.log("I am From Render")
        return (
            <center>
                <div>Hello I am Class {this.state.data}</div>   
            </center>
        )
    }
}

export default Aclasscmp
```

