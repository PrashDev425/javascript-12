# JavaScript Popups

JavaScript provides built-in dialog boxes that allow basic interaction with users.

## Browser built-ins:

|   Method    |          Syntax             |                   Description                   |           Return Value            |
|-------------|-----------------------------|-------------------------------------------------|-----------------------------------|
| `alert()`   | `alert(message)`            | Displays a simple message dialog                | No return value                   |
| `prompt()`  | `prompt(message, default?)` | Displays an input dialog for user input         | `string` or `null` (if cancelled) |
| `confirm()` | `confirm(message)`          | Displays a confirmation dialog with OK / Cancel | `true` (OK) or `false` (Cancel)   |
