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

#### **for...in** Loop

The ``for...in`` loop is used to iterate over the ``keys (property names)`` of an ``object`` or the ``indexes`` of an ``array``.

Syntax:
```js
for (let key in object) 
{
  // Statements
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

#### ``while`` loop

The ``while`` loop executes a block of code as long as the specified condition is true.

Syntax:

```js
while (condition) 
{
  // Statements
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



### Jump Statements (Loop Control Statements)

**Jump statements** are used to control the flow inside loops. They help you stop a loop early or skip a particular iteration.

#### **break** Statement

The ``break`` statement is used to stop a loop immediately. When JavaScript encounters a ``break``, it exits the loop, and the program continues with the next code after the loop.

Syntax:

```js
break; 
```


#### **continue** Statement

The ``continue`` statement is used to skip the current iteration of a loop. When JavaScript sees ``continue``, it jumps directly to the next loop iteration, without executing the remaining statements in the current iteration.

Syntax:

```js
continue;
```
