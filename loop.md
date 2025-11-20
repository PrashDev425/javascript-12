# JavaScript - Loop

A loop in JavaScript is a control structure that repeats a block of code multiple times until a certain condition becomes false.

### ``for`` loop

The ``for`` loop is used when you know in advance how many times the script should run.

Syntax:

```JS
for (initialization; condition; increment/decrement) 
{
  // Statements
}
```

Example:

```JS
for (let x = 0; x <= 10; x++) 
{
  console.log("The number is: "+x);
}
```

### ``while`` loop

The ``while`` loop executes a block of code as long as the specified condition is true.

Syntax:

```JS
while (condition) 
{
  // Statements
}
```

Example:

```JS
let x = 1;
while (x <= 5) 
{
  console.log("The number is: "+x);
  x++;
}
```

### ``do`` ``while`` loop

The ``do...while`` loop - Loops through a block of code once, and then repeats the loop as long as the specified condition is true.The ``do...while`` loop will always execute the block of code once, it will then check the condition, and repeat the loop while the specified condition is true.

Syntax:

```JS
do 
{
  // Statements
} while (condition); 
```

Example:

```JS
let x = 1;
do
{
  console.log("The number is: "+x);
  x++;
} while (x <= 5);
```
