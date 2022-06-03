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




## Appendix
- [Var, Let, and Const – What's the Difference?](https://www.freecodecamp.org/news/var-let-and-const-whats-the-difference/#:~:text=1%20var%20declarations%20are%20globally%20scoped%20or%20function,top%20of%20their%20scope.%20...%20More%20items...%20)
- [Arrow Function](https://www.freecodecamp.org/news/arrow-function-javascript-tutorial-how-to-declare-a-js-function-with-the-new-es6-syntax/)
- [Modern JavaScript](https://www.freecodecamp.org/news/learn-modern-javascript/)
