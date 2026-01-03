# JavaScript - Functions

In ``JavaScript``, a function is a reusable block of code designed to perform a specific task. Functions help organize code, make it reusable, and improve readability.

A function is like a machine:

- You give it input (parameters)
- It performs some actions
- It may return output

## Ways to Create Functions

### A. Function Declaration

```js
function greet() 
{
    document.writeln("Hello!");
}

greet();
```

### B. Function Expression

```js
const greet = function () 
{
    document.writeln("Hello!");
};

greet();
```

## Types of Functions

Based on parameters and return types, functions in JS are classified into 4 types:

| Type   | Parameters | Return Type | Name                          | 
| ------ | ---------- | ----------- | ----------------------------- |
| Type 1 | No         | No          | No parameter, no return value | 
| Type 2 | Yes        | No          | Parameter, no return value    |
| Type 3 | No         | Yes         | No parameter, returns value   |
| Type 4 | Yes        | Yes         | Parameter and returns value   |


```js

function addition() 
{
    let a = 10, b = 5;
    document.writeln(`Addition: ${a} + ${b} = ${a + b} <br>`);
}

function subtraction(a, b) 
{
    document.writeln(`Subtraction: ${a} - ${b} = ${a - b} <br>`);
}

function multiplication() 
{
    let a = 6, b = 7;
    return a * b;
}

function division(a, b) 
{
    if (b !== 0) {
        return a / b;
    } else {
        console.log("Division by zero not allowed!");
        return 0;
    }
}

addition();
subtraction(20, 8);
let product = multiplication();
document.writeln(`Multiplication: 6 * 7 = ${product} <br>`);
let quotient = division(25, 3);
document.writeln(`Division: 25 / 3 = ${quotient.toFixed(2)} <br>`);

```

## Default Parameters

In **JavaScript**, the default value of a function parameter is ``undefined`` if no argument is provided when the function is called. 

However, the ES6 (ECMAScript 2015) feature, known as ``default parameters``, allows you to initialize named parameters with a specific default value directly in the function definition. This value is used if the parameter is missing or explicitly passed as undefined.

```js
function greet(name = "Guest") 
{
    document.writeln("Hello " + name);
}

greet(); // Hello Guest
greet("Ram"); // Hello Ram
```

```js
function volume(l = 10, b = 10, h = 10) 
{
    return l * b * h;
}

document.writeln(volume()); // 1000  → 10 * 10 * 10
document.writeln("<br>" + volume(5)); // 500  → 5 * 10 * 10
document.writeln("<br>" + volume(5, 4)); // 200  → 5 * 4 * 10
document.writeln("<br>" + volume(5, 4, 3)); // 60   → 5 * 4 * 3
```
### Order of Default Parameters

In **JavaScript**, ``default parameters`` must be placed at the end of the parameter list.

```js
function volume(l, b, h = 10) // Correct Order
function volume(l = 10, b, h) // Wrong Order
```

**Reasons:**

- Arguments are assigned from ``left`` to ``right``
- If a default parameter comes before a non-default one, it causes ``ambiguity``

## Higher Order Function

A **Higher Order Function** is a function that does at least one of the following:

- Takes another function as an argument
- Returns a function

### Function as an Argument

```js
function sum(a, b) 
{
    document.writeln("Sum:", a + b);
}

function mul(a, b) 
{
    document.writeln("Product:", a * b);
}

function execute(callback, a, b) 
{
    callback(a, b);
}

execute(sum, 20, 10);
execute(mul, 2, 10);
```

### Function Returning Another Function

```js
function sayHello(name) 
{
    return function () 
    {
        document.writeln("Hello " + name);
    };
}

const greet = sayHello("Ram");
greet(); // Hello Ram
```
