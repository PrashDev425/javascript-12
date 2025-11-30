# Window Console Object

The ``console`` object provides access to the browser's debugging console.


| Method             | Prototype (Signature)                          | Description                                                                     |
|--------------------|------------------------------------------------|---------------------------------------------------------------------------------|
| `assert()`         | `console.assert(condition, message?)`          | Writes an error message if the assertion is false                               |
| `count()`          | `console.count(label?)`                        | Logs the number of times this label has been called                             |
| `error()`          | `console.error(message, ...optionalParams)`    | Outputs an error message                                                        |
| `group()`          | `console.group(label?)`                        | Creates a new inline group (indents following logs)                             |
| `groupCollapsed()` | `console.groupCollapsed(label?)`               | Creates a collapsed inline group                                                |
| `groupEnd()`       | `console.groupEnd()`                           | Exits the current inline group                                                  |
| `info()`           | `console.info(message, ...optionalParams)`     | Outputs an informational message                                                |
| `log()`            | `console.log(message, ...optionalParams)`      | Outputs a message to the console                                                |
| `table()`          | `console.table(tabularData, properties?)`      | Displays structured data as a table                                             |
| `time()`           | `console.time(label?)`                         | Starts a timer                                                                  |
| `timeEnd()`        | `console.timeEnd(label?)`                      | Stops a timer started with `console.time()`                                     |
| `trace()`          | `console.trace(message?)`                      | Outputs a stack trace                                                           |
| `warn()`           | `console.warn(message, ...optionalParams)`     | Outputs a warning message                                                       |
| `clear()`          | `console.clear()`                              | Clears the console                                                              |

**Example:**

```js
// console.assert()
console.assert(5 > 10, "5 is not greater than 10");

// console.count()
console.count("Counter");
console.count("Counter");
console.count("Counter");

// console.error()
console.error("This is an error message");

// console.group()
console.group("Main Group");
console.log("Inside main group");

// console.groupCollapsed()
console.groupCollapsed("Collapsed Group");
console.log("Inside collapsed group");
console.groupEnd(); // end collapsed group
console.groupEnd(); // end main group

// console.info()
console.info("This is an info message");

// console.log()
console.log("A normal log message");

// console.table()
console.table([
    { name: "Alice", age: 25 },
    { name: "Bob", age: 30 }
]);

// console.time() and console.timeEnd()
console.time("Timer Example");
for (let i = 0; i < 1000000; i++) { } // simple loop
console.timeEnd("Timer Example");

// console.trace()
function callTrace() {
    console.trace("Trace message");
}
callTrace();

// console.warn()
console.warn("This is a warning");

//console.clear();
```
