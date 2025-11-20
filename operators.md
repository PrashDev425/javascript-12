# JavaScript - Operators

## Operators
Operators are the foundation of any programming language. Thus the functionality of any programming language is incomplete without the use of operators. We can define operators as symbols that help us to perform specific mathematical and logical computations on operands. In other words, we can say that an operator operates the operands.

For example, consider the below statement:

```JS
c = a + b;
```

Here, `` + ``  is the operator known as addition operator and ``a`` and ``b`` are operands. The addition operator tells the compiler to add both of the operands ``a`` and ``b``.

``JavaScript`` is rich in built-in operators and provides the following types of operators −

* Arithmetic Operator
* Relational Operator
* Logical Operator
* Assignment Operator
* Increment/decrement Operator
* Conditional Operator
* Bitwise Operator

### **Arithmetic Operator**
These are the operators used to perform arithmetic/mathematical operations on operands.

|Operator|       Meaning     | Example |
|:------:|-------------------|---------|
|    +   |      Addition     |  A + B  |
|    −   |    Subtraction    |  A − B  |
|    *   |  Multiplication   |  A * B  |
|    /   |      Division     |  B / A  |
|    %   |Modulus (remainder)|  B % A  |

### **Relational Operator**
These are used for comparison of the values of two operands. For example, checking if one operand is equal to the other operand or not, an operand is greater than the other operand or not etc.

| Operator |            Meaning               | Example |
|:--------:|----------------------------------|:-------:|
|    <     | is less than                     |  a < b  |
|    <=    | is less than or equal to         | a <= b  |
|    >     | is greater than                  |  a > b  |
|    >=    | is greater than or equal to      | a >= b  |
|    ==    | is equal to (value only)         | a == b  |
|    !=    | is not equal to (value only)     | a != b  |
|   ===    | strict equal (value + type)      | a === b |
|   !==    | strict not equal (value + type)  | a !== b |

### **Logical Operator**
Logical Operators are used to combine two or more conditions/constraints or to complement the evaluation of the original condition in consideration. The result of the operation of a logical operator is a boolean value either true or false.

|  Operator      |  Meaning                                               |   Example   |
|:--------------:|--------------------------------------------------------|:-----------:|
|  `&&`(AND)     |True only if both are True otherwise False              |   `a && b`  |
|  `∥`(OR)       |True if either of them are True ,False if all are false |   `a ∥ b`   |
|  `!`(NOT)      |False if it is True,True if it is false                 |     `!a`    |
 
### **Assignment Operator**
Assignment operators are used to assign value to a variable. The left side operand of the assignment operator is a variable and right side operand of the assignment operator is a value. The value on the right side must be of the same data-type of variable on the left side otherwise the compiler will raise an error.

|Operator|         Meaning                                                                        |                    Example                      |
|:------:|----------------------------------------------------------------------------------------|:-----------------------------------------------:|
|   =    |Simple assignment operator. Assigns values from right side operands to left side operand|  ``a = 10;``                                    |
|   +=   |This operator is combination of ‘+’ and ‘=’ operators                                   | ``(a += b)`` can be written as ``(a = a + b)``  |
|   -=   |This operator is combination of ‘+’ and ‘=’ operators                                   | ``(a -= b)`` can be written as ``(a = a - b)``  |
|   *=   |This operator is combination of ‘+’ and ‘=’ operators                                   | ``(a *= b)`` can be written as ``(a = a * b)``  |
|   /=   |This operator is combination of ‘+’ and ‘=’ operators                                   | ``(a /= b)`` can be written as ``(a = a / b)``  |

### **Increment/decrement Operator** 
In ``JavaScript``, the increment operator ``++`` increases the value of a variable by 1. Similarly, the decrement operator ``--`` decreases the value of a variable by 1.

### **Conditional Operator** 
The conditional operator is also known as a ternary operator. The conditional statements are the decision-making statements which depends upon the output of the expression. It is represented by two symbols, i.e., ``?`` and ``:``.

As conditional operator works on three operands, so it is also known as the ternary operator.

The behavior of the conditional operator is similar to the 'if-else' statement as 'if-else' statement is also a decision-making statement.

Syntax:
```JS
variable = <condition> ? <value1> : <value2>; 
```
It can be visualized into if-else statement as:  
```c
if(condition)
{
  variable = value1;
}
else
{
  variable = value2;
}
```
Example:

```JS
x = (a>b) ? a : b;
```
### **Bitwise Operator**
In arithmetic-logic unit (which is within the CPU), mathematical operations like: addition, subtraction, multiplication and division are done in bit-level. To perform bit-level operations in ``JavaScript``, bitwise operators are used.

<table style="width:100%">
  <tr>
    <th>Operators</th>
    <th>Meaning of operators</th>
  </tr>
  <tr>
    <td>&</td>
    <td>Bitwise AND</td>
  </tr>
  <tr>
    <td>|</td>
    <td>Bitwise OR</td>
  </tr>
   <tr>
    <td>^</td>
    <td>Bitwise XOR</td>
  </tr>
  <tr>
    <td>~</td>
    <td>Bitwise complement</td>
  </tr>
   <tr>
    <td><<</td>
    <td>Shift left</td>
  </tr>
  <tr>
    <td>>></td>
    <td>Shift right</td>
  </tr>
</table>