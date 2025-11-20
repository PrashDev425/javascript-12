## JavaScript - Control Structures

Control structure actually controls the flow of execution of a program. Following are the several control structure supported by javascript.

* ``if`` … ``else``
* ``switch`` case
* ``for`` loop
* ``while`` loop
* ``do`` ``while`` loop

### ``if``

``if`` statement is the most simple decision making statement. It is used to decide whether a certain statement or block of statements will be executed or not i.e if a certain condition is true then a block of statement is executed otherwise not.

Syntax:

```JS
if (condition)
{ 
  Statement(s);
} 
```

Example:

```JS
let name = "Prashant";
if (name == "Prashant") 
{
  console.log("Your name is Prashant");
} 
```

### ``if-else``

The ``if`` statement alone tells us that if a condition is ``true`` it will execute a block of statements and if the condition is ``false`` it won’t. But what if we want to do something else if the condition is ``false``. Here comes the ``else`` statement. We can use the ``else`` statement with ``if`` statement to execute a block of code when the condition is ``false``.

Syntax:
```JS
if (condition)
{
  Statement(s);
}
else
{
  Statement(s);
}
```

Example:
```JS
let num = 45;
if (a > 0) 
{
  console.log(num+" is Positive Number");
} 
else 
{
  console.log(num+" is Negetive Number");
}
```
> The block of code following the else statement is executed as the condition present in the if statement is false.

### ``if-else-if``

Here, a user can decide among multiple options. The ``if`` statements are executed from the top down. As soon as one of the conditions controlling the ``if`` is ``true``, the statement associated with that ``if`` is executed, and the rest of the ``else-if`` ladder is bypassed. If none of the conditions are ``true``, then the final ``else`` statement will be executed.

Syntax:

```JS
if (condition)
{
    Statement(s);
}
else if (condition)
{
    Statement(s);
}
.
.
else
{
    Statement(s);
}
```

Example:

```JS
let a = 10; 
let b = 45;
if (a > b) 
{
  console.log(a+" is Greater");
} 
else if (b > a) 
{
  console.log(b+" is Greater");
} 
else 
{
  console.log("Both are Equal");
}
```

### ``switch`` case

The ``switch`` statement is used to perform different actions based on different conditions.

Syntax:

```JS
switch (Expression) 
{
  case (value 1):
  {
    Statements;
    break;
  }
  case (value 2):
  {
    Statements;
    break;
  }
    ...
  default:
  {
    Statements;
  }
}
```

Example:

```JS
let favcolor = "red";
switch (favcolor) 
{
  case ("red"):
  {
    console.log("Your favorite color is red!");
    break;
  }
  case ("blue"):
  {
    console.log("Your favorite color is blue!");
    break;
  }
  case ("green"):
  {
    console.log("Your favorite color is green!");
    break;
  }
  default:
  {
    console.log("Your favorite color is neither red, blue, nor green!");
  }
}
```