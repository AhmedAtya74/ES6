# JavaScript


### Hoisting of var

Hoisting is a JavaScript mechanism where variables and function declarations are moved to the top of their scope before code execution.<br>
This means that if we do this:
``` 
console.log (greeter);
var greeter = "say hello"
```

it is interpreted as this:
```
var greeter;
console.log(greeter); // greeter is undefined
greeter = "say hello"
```


### in case you missed the differences, here they are:

* Var declarations are globally scoped or function scoped while let and const are block scoped.
* Var variables can be updated and re-declared within its scope; let variables can be updated but not re-declared; const variables can neither be updated nor re-declared.
* They are all hoisted to the top of their scope. But while var variables are initialized with undefined, let and const variables are not initialized.
* While var and let can be declared without being initialized, const must be initialized during declaration.



### Rest & Spread Operator

#### Rest

* Used to merge a list of function args into a array
```
myBio = (firstName, lastName, ...otherInfo) => otherInfo

// Invoke myBio function while passing five arguments to its parameters:
res = myBio("Oluwatobi", "Sofela", "CodeSweetly", "Web Developer", "Male");

console.log(res) // ["CodeSweetly", "Web Developer", "Male"]
```
#### Spread

* Used to split up array elements OR object properties
````
myDetails = (first, last, age, gender) => age;

age = myDetails(...['AHMED', 'HASSAN', 22, 'MALE'])

console.log(age); // 22
````


#### Rest & Spread
````
myDetails = (first, last, age, gender, ...aboutEducation) => aboutEducation;


education = myDetails(...['AHMED', 'HASSAN', 22, 'MALE', 'Cairo university','FCAI','CS'])

console.log(education); // ['Cairo university','FCAI','CS']
````


### Destructing 

````
let introduction = ["Hello", "Ahmed"];
let greeting = introduction[0]
let name = introduction[1]

console.log(greeting);//"Hello"
console.log(name);//"Ahmed"

        ||
        ||
        vv

let introduction = ["Hello", "Ahmed"];
let [greeting, name] = introduction;

console.log(greeting);//"Hello"
console.log(name);//"Ahmed"
````

#### Object Destructuring
````
let person = {Name: 'Ahmed', Age:22};

let {Name, Age} = person;

console.log(Name, Age); // Ahmed 22
````

#### Variables declared before being assigned
````
let person = {Name: 'Ahmed', Age:22};

let Name, Age;

{Name, Age} = person;

console.log(Name, Age); // Error

````
##### Fixed by ()
````
let person = {Name: 'Ahmed', Age:22};

let Name, Age;

({Name, Age} = person); <== fixed

console.log(Name, Age); // Ahmed 22

````
 #### Using Default Values
 ````
let person = {Age:22};

let {Name="Ahmed", Age} = person;

console.log(Name, Age); // Ahmed 22
 ````


## Appendix
- [Var, Let, and Const – What's the Difference?](https://www.freecodecamp.org/news/var-let-and-const-whats-the-difference/#:~:text=1%20var%20declarations%20are%20globally%20scoped%20or%20function,top%20of%20their%20scope.%20...%20More%20items...%20)
- [Arrow Function](https://www.freecodecamp.org/news/arrow-function-javascript-tutorial-how-to-declare-a-js-function-with-the-new-es6-syntax/)
- [JavaScript Classes](https://www.freecodecamp.org/news/javascript-classes-how-they-work-with-use-case/)
- [JavaScript Rest vs Spread Operator – What’s the Difference?](https://www.freecodecamp.org/news/javascript-rest-vs-spread-operators/)
- [Modern JavaScript](https://www.freecodecamp.org/news/learn-modern-javascript/)
- [Arguments in JavaScript – What Exactly Is an Argument?](https://codesweetly.com/javascript-arguments#what-is-an-arraylike-object)

