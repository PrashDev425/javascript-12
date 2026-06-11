# JavaScript - Variables & Datatypes 

JavaScript uses variables to store data, and every value in JavaScript has a datatype.


## **Variables in JavaScript**

A variable is a container used to store data values.

JavaScript provides **three** keywords for variable declaration:

### **1. `var`**

-   Old way of declaring variables
-   Function scoped
-   Can be re-declared and updated

### **2. `let`**

-   Modern and recommended
-   Block scoped
-   Can be updated but **cannot be re-declared** in the same scope

### **3. `const`**

-   Block scoped
-   Cannot be updated or re-declared
-   Must be initialized during declaration

### **Example**

``` js
var name = "Ram";
let age = 20;
const PI = 3.14;
name = "Sita"; 
age = 30
PI = 4.67; // Error
```

## **Datatypes in JavaScript**

JavaScript has two categories of datatypes:

-   **Primitive Datatypes**
-   **Non-primitive (Reference) Datatypes**

### **1. Primitive Datatypes**

#### **a) Number**

Represents integer and decimal values.

``` js
let marks = 88;
let price = 99.99;
```

#### **b) String**

Represents text inside quotes.

``` js
let name = "Ram";
let char = 'A';
```

#### **c) Boolean**

Represents true or false.

``` js
let isAdmin = false;
```

#### **d) Undefined**

Variable declared but not assigned.

``` js
let x; // undefined
```

#### **e) Null**

Represents empty or unknown value.

``` js
let empty = null;
```

#### **f) BigInt**

Represents very large integers.

``` js
let big = 12345678901234567890n;
```

#### **g) Symbol**

Represents a unique identifier.

``` js
let sym = Symbol("id");
```

------------------------------------------------------------------------

### **2. Non-Primitive Datatypes**

#### **a) Object**

Stores key--value pairs.

``` js
let user = {
  name: "Ram",
  age: 20
};
```

#### **b) Array**

Stores multiple values.

``` js
let colors = ["red", "blue", "green"];
let marks = [45, 34, 56, 70, 85];
```

#### **c) Function**

Block of reusable code.

``` js
function greet() 
{
  console.log("Hello!");
}
```

------------------------------------------------------------------------

## **Example (All Datatypes Together)**

``` js
let age = 20;                      // Number
let name = "Ram";                  // String
let grade = 'A';                   // Single Character
let isStudent = true;              // Boolean
let x;                             // Undefined
let empty = null;                  // Null

console.log(age);
console.log(name);
console.log(grade);
console.log(isStudent);
console.log(x);
console.log(empty);

console.log(typeof(age));
console.log(typeof(name));
console.log(typeof(grade));
console.log(typeof(isStudent));
console.log(typeof(x));
console.log(typeof(empty));
```

## **Printing output in js**

```js
let name = "Ram";
let age = 25;
console.log("My name is " + name + " and my age is " + age);
console.log("My name is", name, "and my age is", age);
console.log(`My name is ${name} and my age is ${age}`)
console.log("My name is %s and my age is %d", name, age);
```