## JavaScript - Control Structures

Control structure actually controls the flow of execution of a program. Following are the several control structure supported by javascript.

- **Decision Making (Conditional Statements)**
  - ``if``
  - ``if-else``
  - ``if-else-if``
  - ``switch`` cases

- **Looping (Iteration Statements)**
  - ``for`` loop
  - ``for…in`` loop
  - ``for…of`` loop
  - ``while`` loop
  - ``do…while`` loop

- **Jump Statements (Loop Control Statements)**
  - ``break`` – stops the loop immediately
  - ``continue`` – skips the current iteration

### Decision Making (Conditional Statements)

**Decision-making statements** allow JavaScript to execute certain parts of code based on conditions. A condition usually checks whether something is true or false.

#### ``if``

``if`` statement is the most simple decision making statement. It is used to decide whether a certain statement or block of statements will be executed or not i.e if a certain condition is true then a block of statement is executed otherwise not.

Syntax:

```js
if (condition)
{ 
  // Statements;
} 
```

Example:

```js
let age = 20;

if (age >= 18) 
{
    console.log("You are an adult. You can vote.");
}

```

#### ``if-else``

The ``if`` statement alone tells us that if a condition is ``true`` it will execute a block of statements and if the condition is ``false`` it won’t. But what if we want to do something else if the condition is ``false``. Here comes the ``else`` statement. We can use the ``else`` statement with ``if`` statement to execute a block of code when the condition is ``false``.

Syntax:
```js
if (condition)
{
  // Statements;
}
else
{
  // Statements;
}
```

Example:
```js
let num = 45;
if (num % 2 == 0) 
{
    console.log(num + " is Even Number");
} 
else 
{
    console.log(num + " is Odd Number");
}
```
> The block of code following the else statement is executed as the condition present in the if statement is false.

#### ``if-else-if``

Here, a user can decide among multiple options. The ``if`` statements are executed from the top down. As soon as one of the conditions controlling the ``if`` is ``true``, the statement associated with that ``if`` is executed, and the rest of the ``else-if`` ladder is bypassed. If none of the conditions are ``true``, then the final ``else`` statement will be executed.

Syntax:

```js
if (condition)
{
  // Statements;
}
else if (condition)
{
  // Statements;
}
.
.
else
{
  // Statements;
}
```

Example:

```js
let a = 10; 
let b = 45;
if (a > b) 
{
    console.log(a + " is Greater");
} 
else if (b > a) 
{
    console.log(b + " is Greater");
} 
else 
{
    console.log("Both are Equal");
}
```

#### ``switch`` case

The ``switch`` statement is used to perform different actions based on different conditions.

Syntax:

```js
switch (Expression) 
{
    case (value 1):
    {
        // Statements;
        break;
    }
    case (value 2):
    {
        // Statements;
        break;
    }
    ...
    default:
    {
        // Statements;
    }
}
```

Example:

```js
let marks = 78;   // Change this to test

switch (true)
{
    case (marks >= 90 && marks <= 100):
    {
        console.log("Grade: A");
        break;
    }
    case (marks >= 80 && marks < 90):
    {
        console.log("Grade: B");
        break;
    }
    case (marks >= 70 && marks < 80):
    {
        console.log("Grade: C");
        break;
    }
    case (marks >= 60 && marks < 70):
    {
        console.log("Grade: D");
        break;
    }
    case (marks >= 50 && marks < 60):
    {
        console.log("Grade: E");
        break;
    }
    case (marks >= 0 && marks < 50):
    {
        console.log("NG");
        break;
    }
    default:
    {
        console.warn("Invalid Marks: Marks Range [0 - 100]");
    }
}

```

### Looping (Iteration Statements)

**Looping** allows you to repeat a block of code multiple times. Loops are useful when you need to perform the same task again and again.

#### ``for`` loop

The ``for`` loop is used when you know in advance how many times the script should run.

Syntax:

```js
for (initialization; condition; increment/decrement) 
{
  // Statements
}
```

Example:

```js
for (let x = 0; x <= 20; x++) 
{
    console.log("The number is: " + x);
}
for (let x = 0; x <= 20; x += 2) 
{
    console.log("Even: " + x);
}
for (let x = 1; x <= 20; x += 2) 
{
    console.log("Odd: " + x);
}
```

#### **for...in** Loop

The ``for...in`` loop is used to iterate over the ``keys (property names)`` of an ``object`` or the ``indexes`` of an ``array``.

Syntax:
```js
for (let key in object) 
{
  // Statements
}
```

Example:
```js
const person = { 
  name: "John",
  age: 25, 
  country: "Nepal" 
};

for (let key in person) 
{
    console.log(key + ": " + person[key]);
}

const fruits = ["Apple", "Banana", "Mango"];

for (let index in fruits) 
{
    console.log(index, fruits[index]);
}
```

### **for...of** Loop

The ``for...of`` loop is used to iterate over values of an iterable (Array, String, Map, Set, etc.)

Syntax:
```js
for (let value of iterable) 
{
  // Statements
}
```

Example:

```js
const colors = ["Red", "Green", "Blue"];

for (let color of colors) 
{
    console.log(color);
}

for (let char of "JavaScript") 
{
    console.log(char);
}
```

#### ``while`` loop

The ``while`` loop executes a block of code as long as the specified condition is true.

Syntax:

```js
while (condition) 
{
  // Statements
}
```

Example:

```js
let maxRetries = 5;
let attempt = 0;
let connected = false;

while (attempt < maxRetries && connected == false) 
{
    attempt++;
    console.log(`Attempt ${attempt}: Trying to connect...`);
    // Simulate random connection success (20% chance)
    let success = Math.random() < 0.2;
    if (success == true) 
    {
      console.log("Connected successfully!");
      connected = true;
    } 
    else 
    {
      console.log("Connection failed. Retrying...\n");
    }
    // -----------------------------------------------
}

if (!connected) {
    console.log("Max retries reached. Could not connect.");
}

```

#### ``do`` ``while`` loop

The ``do...while`` loop - Loops through a block of code once, and then repeats the loop as long as the specified condition is true.The ``do...while`` loop will always execute the block of code once, it will then check the condition, and repeat the loop while the specified condition is true.

Syntax:

```js
do 
{
  // Statements
} while (condition); 
```

Example:

```js
let password;
do 
{
    password = prompt("Enter password:");
} while (password !== "1234");
console.log("Access Granted!");
```



### Jump Statements (Loop Control Statements)

**Jump statements** are used to control the flow inside loops. They help you stop a loop early or skip a particular iteration.

#### **break** Statement

The ``break`` statement is used to stop a loop immediately. When JavaScript encounters a ``break``, it exits the loop, and the program continues with the next code after the loop.

Syntax:

```js
break; 
```

Example:

```js
const correctPin = "5832"; // the pin we want to find

for (let i = 0; i <= 9999; i++) 
{
    // convert number to a 4-digit string
    const attempt = i.toString().padStart(4, "0");
    console.log(`Trying: ${attempt}`);
    if (attempt === correctPin) 
    {
        console.log(`PIN found: ${attempt}`);
        break;
    }
}
```

#### **continue** Statement

The ``continue`` statement is used to skip the current iteration of a loop. When JavaScript sees ``continue``, it jumps directly to the next loop iteration, without executing the remaining statements in the current iteration.

Syntax:

```js
continue;
```

Example:

```js
const fields = ["John", "", "Dog", "", "Nepal", "", "", "Apple"];

for (let i = 0; i < fields.length; i++) 
{
    if (fields[i] === "") 
    {
        continue; // skip empty fields
    }
    console.log(`Processing index ${i}:`, fields[i]);
}
```
