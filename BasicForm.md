## Making a Basic Form 
![](https://github.com/itzsnehasis/Reactjs/blob/main/Gallery/CCxO5DVEQI.gif)

* Setting up the BasicForm Component 
```js
//in BasicForm.js

import { useState } from "react"

function BasicForm() {
    const [name, setName]= useState("")
    const [class_, setClass]= useState("")
    const [gender, setGender]= useState("")
    const [address, setAddress]= useState("")
    const [tnc, setTnc]= useState(false)
    function getformData(e) {
        e.preventDefault()
        console.log(name)
        console.log("____")
        console.log(class_)
        console.log("____")
        console.log(gender)
        console.log("____")
        console.log(address)
        console.log("____")
        console.log(tnc)
    }
    return (
        <center>
            <h1>Basic Form</h1>
            <br/>
            <form onSubmit={getformData}>
                <table border="2px black">
                    <tr>
                        <td>Name</td>
                        <td><input type="text" onChange={event=>setName(event.target.value)}/></td>
                    </tr>
                    <tr>
                        <td>Class</td>
                        <td>
                            <select onChange={event=>setClass(event.target.value)}>
                                <option>Select Class</option>
                                <option>XII</option>
                                <option>XI</option>
                                <option>X</option>
                            </select>
                        </td>
                    </tr>
                    <tr>
                        <td>Gender</td>
                        <td>
                            <input type="radio" name="gender" value="male" onChange={event=>setGender(event.target.value)} />
                            <label>Male</label>
                            <input type="radio" name="gender" value ="female" onChange={event=>setGender(event.target.value)} />
                            <label>Female</label>
                        </td>
                    </tr>
                    <tr>
                        <td>Address</td>
                        <td><textarea style={{width: "139px", height: "30px"}} onChange={event=>setAddress(event.target.value)}></textarea></td>
                    </tr>
                </table>
                <input type="checkbox" onChange={event=>setTnc(event.target.checked)}/><span>Accept Terms and condition</span>
                <br/>
                <br/>
                <button type="submit">Submit</button>
            </form>
        </center>
    )
}

export default BasicForm
```
