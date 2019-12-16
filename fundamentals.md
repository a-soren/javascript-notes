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


### Facts:
* The concept of calling a function is often called **invoking a function**.

* Use `console.log()` if we want to see a result in our web console.

* The values that we passed `(2, 4)` are **arguments** & the function received those arguments as **parameters** `(a, b)` in the exact order they were called.
   * *The name of the parameter doesn't matter syntactically* **
   
* Anything written after a return statement **will not execute**. 
 * The return statment will terminate the function after running the line of statements within it.
 <br /> <br />
 <hr />
 
 
### Hoisting : the concept of putting a function higher in the execution order for later.

JavaScript takes 2 passes over your code:

**1st pass:** 
* builds up references to all of our code ;
* declaring variables and functions and the like.
* The compiler is made aware of the function declaration and adds it to the top of the execution order for your code. 


**2nd pass:** 
* applies values to the references that were found, thus actually running the code.

**Function declarations can be invoked before they are defined!**
```
// This code is valid above the definition!
console.log(add(2,4)) // 6 

function add(a,b){ 
 return a + b;
} 
```
Hoisting applies to function declarations and **not** function expressions or arrow functions.
 <br /> <br />
 <hr />
 
 
 
 
 
 ## Function Expressions
 
* A variable is used to store the function for later use
* Anonymous functions are used
* Function expressions are not hoisted. They can only be invoked after a definition has been placed in the execution stack.

```
const add = function(a,b){ 
 return a + b;
} 
console.log(add(2,4)) // 6 
```

* The above function doesn't actually have a name; 
* referred to as an anonymous function.
* we have more control over our code now.
* we can tell it when to do its job easier. 
* We can place functions within functions easier without having to name them. 
 <br />
 <hr />
 

### Arrow Function Expressions: fancy looking function expressions with a major feature removed, the `this` keyword ("Syntatical Sugar")

```
// function expression syntax
// const add = function(a,b) { 
//  return a + b;
// } 

// arrow function expression syntax
const add = (a,b) => { 
 return a + b;
} 
console.log(add(2,4)) // 6 
```

* function keyword removed
*  => token added behind the parameters.

```
// streamlined arrow syntax
const add = (a,b) => a + b; 

console.log(add(2,4)) // 6 
```

* no longer are required to use the return keyword - because it’s implied!
* do not need our {} because they, too, are redundant in the rules of arrow functions.
* great to use with array methods but not for everything 
 <br />
 <hr />
 
