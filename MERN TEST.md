# MERN Questions:

1. Which of the following attributes is used to open an hyperlink in new tab? : `<target>`

2. Which tag is used to add an header in HTML5 table? : `<th>`

3. The correct precedence of the operators in Javascript is () [] . ++

4. `indexOf(c)` returns the first occurrence of char c

5. All the values false , undefined , ‘ ’, 0 , NaN represent falsy values in javascript

6. All the values {},[].true, a number , non empty strings represent truthy values in javascript ( -> Even 'false' is true coz it's a non-empty string )

7. `strict` in js:

---

Here is the explanation of strict mode in JavaScript, formatted in Markdown:

````markdown
# JavaScript Strict Mode

Strict mode is a feature in JavaScript that helps in catching common coding errors and improving performance. It makes JavaScript behave in a more predictable and safer way. It was introduced in ECMAScript 5 (ES5).

## Enabling Strict Mode

To enable strict mode, add the following line at the beginning of your script or function:

```javascript
"use strict";
```
````

### Global Strict Mode

When placed at the top of a script file, it applies to the entire script.

```javascript
"use strict";

var x = 3.14;
```

### Function Strict Mode

You can also enable strict mode within a specific function:

```javascript
function myFunction() {
  "use strict";
  var y = 42;
}
```

## Key Features of Strict Mode

Here are some of the things that change when using strict mode:

### 1. Eliminates `this` Coercion

In strict mode, the value of `this` is not automatically set to the global object when inside a function. Instead, it remains `undefined`.

**Example:**

```javascript
function myFunction() {
  console.log(this); // undefined in strict mode
}

myFunction();
```

Without strict mode, `this` would refer to the global object (in a browser, `window`).

### 2. Disallows Duplicate Parameter Names

In strict mode, you cannot have duplicate parameter names in a function definition.

**Example:**

```javascript
function myFunction(a, a) {
  console.log(a);
}
// SyntaxError: Duplicate parameter name not allowed in this context
```

Without strict mode, JavaScript allows duplicate parameters, but only the last one is used.

### 3. Prevents Assigning to Read-Only Properties

In strict mode, assigning to a read-only property will throw an error.

**Example:**

```javascript
"use strict";

const obj = {};
Object.defineProperty(obj, "name", {
  value: "Alice",
  writable: false,
});

obj.name = "Bob"; // TypeError: Cannot assign to read only property 'name'
```

Without strict mode, the assignment would silently fail.

### 4. Prohibits `with` Statement

The `with` statement is forbidden in strict mode, as it can lead to ambiguous code and difficulties in debugging.

**Example:**

```javascript
"use strict";
with (Math) {
  console.log(sin(90));
}
// SyntaxError: Strict mode code may not include a with statement
```

### 5. Eliminates `eval` and `arguments` Modifications

In strict mode, you cannot use `eval` or `arguments` to create new variables, nor can you assign to them.

**Example:**

```javascript
"use strict";

eval("var x = 2"); // Throws SyntaxError
arguments[0] = 5; // Throws TypeError
```

### 6. Makes `eval()` and `arguments` Safer

In strict mode, variables declared in `eval()` do not leak out into the surrounding scope.

**Example:**

```javascript
"use strict";

eval("var y = 10");
console.log(y); // ReferenceError: y is not defined
```

Without strict mode, `y` would be available outside of `eval`.

---

8. What is the type of variable data declared below const data=[ ]?  
   The variable data represents an Object in JavaScript

9. An object is an unordered collection of properties each of which has a name and value

10. Method used to create objects in javascript

    - A new keyword
    - B object.create()

11. Both the rest parameter and the spread operator have the same syntax

12. What will be the output of the following code snippet const arr=[1,2,3,4,5] console.log(...arr)  
    A | [1 2 3 4 5]  
    B | ...[1 2 3 4 5]  
    `C |  1 2 3 4 5 `  
    D | ...1 2 3 4 5

13. The text-decoration: the overline property is used to sets many kinds of text-decoration. The text-decoration may include many values such as underline, overline, line-through, etc
14. The order property in CSS which is used responsibly for the order of each flexible item in relation to other items inside the flexible container. If the element is not flexible then item then this property does not exist anymore.
15. The order property in CSS which is used responsibly for the order of each flexible item in relation to other items inside the flexible container. If the element is not flexible then item then this property does not exist anymore.

16. The calc() function in CSS is inbuilt that is used to perform calculations based on the property of CSS. It takes only parameters as expressions.
17. The background-origin is a property that is defined in CSS that helps to set the background images of web pages. It helps to set the origin images. By default, this property sets the background image origin to the upper-left corner of the screen of the webpage.
18. The total number of columns in the bootstrap grinding system is 12. On one page you can make the grid in groups either in 4*3 and 3*4 etc but not greater than 12.

19. The .navbar-inverse is bootstrap class is used to create a black navigation bar Here inverse takes the value as black.

```
Do this again (Bootstrap) :
https://www.geeksforgeeks.org/quizzes/bootstrap-quiz-set-1/

```
