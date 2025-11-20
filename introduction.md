# JavaScript - Introduction

## Introduction

``JavaScript`` is a lightweight, cross-platform, and interpreted scripting language used to make webpages interactive (e.g., having complex animations, clickable buttons, popup menus, etc.). It is well-known for the development of web pages, many non-browser environments also use it.

## Embedding JavaScript in HTML

JavaScript can be added to your HTML file in two ways:

* Internal JS
* External JS

### **Internal JS:** 

We can add JavaScript directly to our HTML file by writing the code inside the ``<script>`` tag. The ``<script>`` tag can either be placed inside the ``<head>`` or the ``<body>`` tag according to the requirement.

Syntax:

```HTML
<script>
    // JavaScript Code
</script>
```
Example:

```HTML 
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Example</title>
</head>
<body>
    <script>
        console.log("This is JavaScript");
    </script>
</body>
</html>
```

### **External JS:** 

In order to accommodate larger scripts or scripts that will be used across several pages, JavaScript code generally lives in one or more js files that are referenced within HTML documents, similarly to how external assets like CSS are referenced.

The benefits of using a separate JavaScript file include:

* Separating the HTML markup and JavaScript code to make both more straightforward.
* Separate files makes maintenance easier.
* When JavaScript files are cached, pages load more quickly.

We can write JavaScript code in other file having an extension ``.js`` and then link this file inside the ``<head>`` tag of the HTML file in which we want to add this code.

How to link:

```HTML
<script src="js file path"></script>
```

Example:

Folder Structure

```
Example2
    ├──index.html
    └──js
        └── logic.js

```

**Content of ``index.html`` :**

```HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <script src="js/logic.js"></script>
    <title>Example2</title>
</head>
<body>
    <script>
        printdate();
    </script>
</body>
</html>
```

**Content of ``logic.js`` :**

```JS
function printdate()
{
    let d = new Date();
    document.body.innerHTML = "<h1>Today's date is " + d + "</h1>";
}
```

## Using Script Tag

The ``<script>`` tag is used to embed a client-side script (JavaScript).

The ``<script>`` element either contains scripting statements, or it points to an external script file through the src attribute.

Example:

```HTML
<script>
document.getElementById("demo").innerHTML = "Hello JavaScript!";
</script>
```

## NoScript Tag


The ``<noscript>`` tag defines an alternate content to be displayed to users that have disabled scripts in their browser or have a browser that doesn't support script.

The ``<noscript>`` element can be used in both ``<head>`` and ``<body>``. When used inside ``<head>``, the ``<noscript>`` element could only contain ``<link>``, ``<style>``, and ``<meta>`` elements.

Example:

```HTML
<script>
document.write("Hello World!")
</script>
<noscript>Your browser does not support JavaScript!</noscript>
```

