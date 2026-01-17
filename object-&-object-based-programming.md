# Object and Object-Based Programming in JavaScript

## Object

An **object** is a collection of key–value pairs. Keys are called **properties**, and values can be any data type.

### Creating object using Object Literal

```js
const objectName = {
    // -------- property / state --------
    property1: value1,
    property2: value2,
    // -------- methods -----------------
    methodName: function () {
        // code
    }
};
```

```js
const student = {
    name: "Ram",
    age: 20,  
    course: "IT", 
    isMarried: false,
    greet: function () { 
        document.write("Hello, my name is " + this.name + "<br>");
    }
};

document.write(student.name + "<br>");
document.write(student.age + "<br>");
document.write(student.course + "<br>");
document.write(student.isMarried + "<br>");
student.greet();

```

### ``this`` Operator

In **JavaScript**, ``this`` is a keyword that refers to the object that is currently calling a function. When ``this`` is used inside an object’s method, it refers to that object.

```js
const obj = {
    value: 20,
    display: function () {
        document.write(this.value);
    }
};

obj.display();
```

## Object-Based Programming

**Object-based programming** is a programming paradigm centered on the concept of **objects** that **encapsulate data (attributes)** and **behavior (methods)** into a single unit. 

JavaScript supports object-based programming, where programs are built around objects.

- An ``object`` is a collection of:
    - **Properties (data/attributes)** : describe the ``object``
    - **Methods (functions)** : define the ``object’s`` behavior

Unlike full **Object-Oriented Programming (OOP)**, object-based programming does not require all OOP features like:

- Inheritance
- Polymorphism
- Abstraction
- Encapsulation in the strict sense (private/protected access)

### Encapsulation in Object-Based Programming

Encapsulation in object-based programming means binding data (properties) and related functions (methods) into a single object and controlling access to that data.

### Tasks

#### Task 1 : Counter

Write a JavaScript program using  **object-based programming (Object Literal)** to implement a counter with the following features:

- The object should have a property to store the counter value.

- Provide a method to increment the counter by ``1``.

- Provide a method to decrement the counter by ``1``, but the value should not go below ``0``.

- Provide a method to reset the counter value to ``0``.

- Provide a method to display the current counter value.

- Demonstrate the working of the counter by calling the methods in proper sequence.

```js
const couter = {
    // -------- property / state --------
    count: 0,
    // -------- methods -----------------
    increment: function () {
        this.count++;
    },
    decrement: function () {
        if (this.count > 0) {
            this.count--;
        }
    },
    reset: function () {
        this.count = 0
    },
    display: function () {
        document.write("Current counter value:" + this.count + "<br>");
    }
}

couter.display();
couter.increment();
couter.increment();
couter.increment();
couter.increment();
couter.display()
couter.reset();
couter.display();
```

#### Task 2 : Bank Account 

Write a JavaScript program using **object-based programming (Object Literal)** to create a Bank Account with the following features:

- The object should have a property to store the account balance.

- A method to deposit a given amount into the account.

- A method to withdraw a given amount from the account (the balance should not become negative).

- A method to reset the account balance to zero.

- A method to display the current account balance.

- Demonstrate the working of the bank account by calling all methods.

```js
const bankAccount = {
    // -------- property / state --------
    balance: 0,

    // -------- methods -----------------
    deposit: function (amount) {
        this.balance += amount;
    },

    withdraw: function (amount) {
        if (amount <= this.balance) {
            this.balance -= amount;
        } else {
            document.write("Insufficient balance<br>");
        }
    },

    reset: function () {
        this.balance = 0;
    },

    display: function () {
        document.write("Current Balance: " + this.balance + "<br>");
    }
};

// -------- method calls ---------------
bankAccount.display();
bankAccount.deposit(1000);
bankAccount.deposit(500);
bankAccount.display();
bankAccount.withdraw(300);
bankAccount.display();
bankAccount.reset();
bankAccount.display();
```

#### Task 3 : School Bus Passenger Counter

**Requirements:**

- Create a constant named `MAX_SEATS` to store the maximum seating capacity of the bus.

- Create an object named `bus`.

- The object should have:
  - `routeName` → name of the bus route  
  - `passengers` → initial value `0`

- The object should include the following methods:
  - `board()` → increases passengers by `1` **only if seats are available**
  - `exit()` → decreases passengers by `1` (**passengers should not be negative**)
  - `resetPassengers()` → sets passengers to `0`
  - `display()` → shows route name, passenger count, and maximum seats

- Call the methods to demonstrate the working of the object.

> Do Yourself
