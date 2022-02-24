# Primitive Datatypes

1. String
2. Boolean
3. Undefined
4. Null
5. Number
6. BigInt
7. Symbols

## String
Strings can be declared in quotes, double quotes and backticks
Strings are immutables in JS.

```
 const str = "Sample String";
```

```
const str = `Sample
    String 
    in multiple lines
    `;
```
## Boolean
Can either be true or false 

``` 
    const a = 20;
    const b = 20;

    Boolean(a+b) -> true
    Boolean('true') -> true
    Boolean([]) -> true
    Boolean({}) -> true

    Boolean('') -> false
    Boolean() -> false
    Boolean(undefined) -> false
    Boolean(null) -> false
```

## Undefined
Any Javascript variable when it is declared, it is immedietly given an undefined value.
Is false

## Null
Any Javascript variable that intentinally doesnt have a value is assigned null.
Is falsy

## Number
Used to represent number in general . 
Any value lesser than Number.MAX_SAFE_INTEGER and
Number.MIN_SAFE_INTEGER

## BigInt
Any number that exceeds memory allocation more than 64 bits intended for a number can be assigned as a bigint.
Used to represent numbers that is outside the range for the Number primitive type.
Can be binary, octal, hexadecimal.

BigInts can be used in operations like +, -, *, %

```
    typeof (1000n) -> bigint
    10n == 10 -> True
    10n === 10 -> False
```

Can be compared with numbers.
We can sort arrays of numbers and bigints

## Symbols
