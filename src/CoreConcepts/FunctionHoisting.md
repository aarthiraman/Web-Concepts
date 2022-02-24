# Function Hoisting
Functions are similar to variables. A normal function gets hoisted and hence 
it can be called after they are declared. 
A normal function when declared is an anonymous function.

Example
```
aFunc(4, 5);
function aFunc (a,b) {
    console.log(a);
    console.log(b);
}

```

Output
'''
    4
    5
'''

## Function Expression
1) A function expression is hoisted but throws a reference error 
when it gets called before the declaration.
2) It is not an anonymous function and can be reffered through the 

Example
```
aFunc(4, 5);
const aFunc = function(a,b) {
    console.log(a);
    console.log(b);
}
```

Output
```
Uncaught ReferenceError: aFunc1 is not defined
```

