# How to make a component ... 
1. Make a file App.js in src folder
2. follow this structure to make a function component in App.js
```js
function App() {
  return (
    <div>
      Hello I am a component
    </div>
  );
}

export default App;
```
3. If you wanna use this component in any other place in your project
   * First Import it by `import App from './App'`
   * Just Use it With `<App/>`
```js
import App from './App';

ReactDOM.render(
  <React.StrictMode>
     <App />  {/*using the component like a html tag*/}
  </React.StrictMode>,
  document.getElementById('root')
);
reportWebVitals();
```
