# JavaScript Popups

JavaScript provides built-in dialog boxes that allow basic interaction with users.

## Browser built-ins:

|   Method    |          Syntax             |                   Description                   |           Return Value            |
|-------------|-----------------------------|-------------------------------------------------|-----------------------------------|
| `alert()`   | `alert(message)`            | Displays a simple message dialog                | No return value                   |
| `prompt()`  | `prompt(message, default?)` | Displays an input dialog for user input         | `string` or `null` (if cancelled) |
| `confirm()` | `confirm(message)`          | Displays a confirmation dialog with OK / Cancel | `true` (OK) or `false` (Cancel)   |

## Example:

```js
alert('Hello! This is an alert.');

const name = prompt('What is your name?', 'Guest');
alert('Nice to meet you, ' + name + '!');

const ok = confirm('Do you want to continue?');
if (ok == true) 
{
    alert('You chose to continue.');
} 
else 
{
    alert('You chose to cancel.');
}
```

## numeric prompt (safe parsing)

```js
const input = Number(prompt('Enter a number between 1 and 10:'));
if (Number.isNaN(input)) 
{
    console.log('Not a number');
} else 
{
    console.log('You entered', n);
}
```
