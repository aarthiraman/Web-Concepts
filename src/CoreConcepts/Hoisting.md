# Hoisting
When the engine parses through the code during the creation phase,
the variable declarations are moved to the top of the scope in which 
they are declared.

## Variable Hoisting
1. With hoisting variables only the declarations gets moved to the top
of the code block
2. Definition of the variables only happens when the code is executed.
3. Until that it is given a default value which is undefined

In the below problem all the variable declarations gets moved to the top.

```
  var a = 'hello'
  console.log('value of a is', a)
  var a;
  var b = 10;
  var b;
  console.log('value of b is', b)
  var c = 10
  var c = 12
  console.log('value of c is', c)
```

```
value of a is hello
value of b is 10
value of c is 12
```

### NOTE: 
1. Anything declared as var gets a value undefined assigned to it initially.
2. A variable when it gets assigned a value and then gets redeclared preserves the initial value.

## let and const
let and const variables get hoisted but they dont get initialized with a value
Hence if it gets used before its definition it would throw a reference error.