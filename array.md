# Arrays in js

An array is a fundamental data structure in computing, representing an ordered collection of elements stored together in a single variable, accessed via a numeric index starting from ``0``.

An array in JavaScript is a special variable that can store multiple values in a single variable.


```
         Index →
         
  0    1    2    3    4
+----+----+----+----+----+
| 10 | 20 | 30 | 40 | 50 |
+----+----+----+----+----+

Size: 5 
First Index: 0
Last Index: (Size - 1) = 4
```

## Initialization

You can create a empty array

```js
let arr = [];
```

OR

You can assign values directly when declaring an array.

```js
int arr = [10, 20, 30, 40, 50];
```

## Example

**Using Array:**

```c
let number = [];

number[0] = 10;
number[1] = 20;
number[2] = 30;
number[3] = 40;
number[4] = 50;

document.write("number[0] = " + number[0] + "<br>");
document.write("number[1] = " + number[1] + "<br>");
document.write("number[2] = " + number[2] + "<br>");
document.write("number[3] = " + number[3] + "<br>");
document.write("number[4] = " + number[4] + "<br>");
```

**Programatically [using Array]:**

```c
let number = [];
let size = 5;

for (let i = 0; i < size; i++) {
    number[i] = (i + 1) * 10;
}

for (let i = 0; i < number.length; i++) {
    document.write("number[" + i + "] = " + number[i] + "<br>");
}
```

## ``length`` Property

The ``length`` property returns the number of elements in an array.

```js
int arr = [10, 20, 30, 40, 50];
document.write("Length: " + arr.length) // 5
```

## Array Methods :``push()`` and ``pop()``

| Method   | Prototype (Syntax)                    | Description                                          | Return Value            |
| -------- | ------------------------------------- | ---------------------------------------------------- | ----------------------- |
| `push()` | `array.push(element1, element2, ...)` | Adds one or more elements to the **end** of an array | New length of the array |
| `pop()`  | `array.pop()`                         | Removes the **last** element from an array           | The removed element     |

**Example:**

```js
let arr = [10, 20];
arr.push(30);
console.table(arr);
let last = arr.pop();
console.log("Popped : " + last);
console.table(arr);
```

## Tasks

### 1. Simple Search (Linear Search)

In computer science, linear search or sequential search is a method for finding an element within a list. It sequentially checks each element of the list until a match is found or the whole list has been searched.

The ``linearSearch()`` function returns an integer value that represents either:

- the index of the searched element, or

- ``-1`` if the element is not present in the array.

```js
function linearSearch(arr, key) 
{
  for (let i = 0; i < arr.length; i++) 
  {
    if (arr[i] === key) 
    {
      return i;
    }
  }
  return -1;
}

let numbers = [5, 15, 25, 35, 45];
let result = linearSearch(numbers, 25);
if (result !== -1) 
{
  document.write("Element found at index: " + result);
} 
else 
{
  document.write("Element not found);
}
```


### 2. Sum of Array

```js
function sumOfArray(arr) 
{
  let sum = 0;
  for (let i = 0; i < arr.length; i++) 
  {
    sum += arr[i];
  }
  return sum;
}

let numbers = [10, 20, 30, 40, 50];
let result = sumOfArray(numbers);
document.write("Sum of array elements: "+ result);
```

### 3. Min, Max, Avg & Reverse of Array

```js
min(arr)
max(arr)
avg(arr)
reverse(arr) // using inverse loop and push()
```

> Do Yourself
