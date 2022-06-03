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







## Appendix
- [Var, Let, and Const – What's the Difference?](https://www.freecodecamp.org/news/var-let-and-const-whats-the-difference/#:~:text=1%20var%20declarations%20are%20globally%20scoped%20or%20function,top%20of%20their%20scope.%20...%20More%20items...%20)
