# JavaScript Fundamentals

## Functions : Used to execute the code. 
<br />

```
// Define our function declaration 

function add(a,b){ 

 return a + b;
} 

// Invoke the function add

console.log(add(2,4)) // 6 
```
<br />

* The concept of calling a function is often called **invoking a function**.

* Use `console.log()` if we want to see a result in our web console.

* The values that we passed `(2, 4)` are **arguments** & the function received those arguments as **parameters** `(a, b)` in the exact order they were called.
   * *The name of the parameter doesn't matter syntactically* **
   
* Anything written after a return statement **will not execute**. 
 * The return statment will terminate the function after running the line of statements within it.
 <br />
 
### Hoisting : the concept of putting a function higher in the execution order for later
