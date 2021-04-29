# What is Props ?
Props is a special keyword in React, which stands for properties and is being used for passing data from one component to another.

# Example of using Props 
1. Ok so let App.js is a Component
```js
import Student from './Student'

function App() {
  return (
    <div>
      <Student name={snehasis} email={snehasis@test.com}/>
    </div>
  );
}

export default App;
```
* Here Student is an another component 
* Now we are calling and sending data to student component at the same time by `<Student name={snehasis} email={snehasis@test.com}/>`
* we are calling Student so we have to imported the Student by `import Student from './Student'`
2. Now How We can Access those data in student component and print them 
```js
function Student(props){
    return(
        <center>
            <div>Name: {props.name}, EMail: {props.email}</div>
        </center>
    );
}
export default Student;
```
