# Variables, Data Types, Input, Output, and Operators

## What We Will Learn

In this class, we will start learning JavaScript. We will learn how to store information, work with different types of data, take input from users, display output, and perform calculations.

## 1. What Is a Variable?

A variable is a named place where we store information in a program.

```javascript
let studentName = "Ali";
let age = 20;
let city = "Karachi";

console.log(studentName);
console.log(age);
console.log(city);
```

- `let` creates a variable.
- `studentName`, `age`, and `city` are variable names.
- The values are the information stored in the variables.
- `console.log()` displays information in the console.

## 2. Using `let` and `const`

Use `let` when you may need to change a value later.

```javascript
let score = 50;
console.log(score);

score = 80;
console.log(score);
```

Use `const` when you do not plan to assign a new value to the variable.

```javascript
const country = "Pakistan";
console.log(country);
```

You cannot reassign a `const` variable:

```javascript
const country = "Pakistan";
country = "Turkey"; // This causes an error
```

**Remember:**
- Use `let` when the value may change.
- Use `const` when the variable should not be reassigned.
- Avoid using `var` in new beginner projects; learn `let` and `const` first.

## 3. Variable Naming Conventions

Variable names should be clear and meaningful.

```javascript
let firstName = "Ahmed";
let studentAge = 21;
let totalMarks = 450;
```

Basic naming rules:
- A variable name can contain letters, numbers, `_`, and `$`.
- A variable name cannot start with a number.
- Do not use spaces in variable names.
- JavaScript variable names are case-sensitive. `age` and `Age` are different.
- Do not use JavaScript reserved words as variable names.
- Use meaningful names that explain what the variable stores.
- A common style is **camelCase**: the first word starts with a small letter and each following word starts with a capital letter.

## 4. JavaScript Data Types

A data type tells us what kind of value a variable contains.

### String

A string is text. We can write it using single or double quotes.

```javascript
let studentName = "Ali";
let city = 'Karachi';

console.log(studentName);
console.log(city);
```

### Number

A number can be an integer or a decimal.

```javascript
let age = 20;
let price = 99.50;

console.log(age);
console.log(price);
```

### Boolean

A Boolean value can only be `true` or `false`.

```javascript
let isStudent = true;
let hasLicense = false;

console.log(isStudent);
console.log(hasLicense);
```

### `null`

`null` means we intentionally set a variable to have no value.

```javascript
let selectedColor = null;
console.log(selectedColor);
```

### `undefined`

`undefined` usually means a variable has been declared but no value has been assigned.

```javascript
let userEmail;
console.log(userEmail);
```

### Quick Data Type Summary

| Data type | Example | Meaning |
|---|---|---|
| String | `"Hello"` | Text |
| Number | `25` or `10.5` | Numeric value |
| Boolean | `true` or `false` | True/false value |
| Null | `null` | Intentionally empty value |
| Undefined | `undefined` | No value assigned |

## 5. Using `typeof`

The `typeof` operator helps us check the type of a value.

```javascript
let name = "Ahmed";
let age = 25;
let isStudent = true;

console.log(typeof name);
console.log(typeof age);
console.log(typeof isStudent);
```

Output:

```text
string
number
boolean
```

You can also check these values:

```javascript
console.log(typeof null);      // object (a historical JavaScript behaviour)
console.log(typeof undefined); // undefined
```

**Important:** JavaScript returns `"object"` for `typeof null`. This is a known historical behaviour of the language.

## 6. Taking User Input with `prompt()`

The `prompt()` function displays an input box and asks the user to enter information.

```javascript
let userName = prompt("Please enter your name:");
console.log(userName);
```

You can use the entered value in a message:

```javascript
let userName = prompt("Please enter your name:");
console.log("Welcome " + userName);
```

**Important:** The value returned by `prompt()` is a string, even if the user enters a number. Convert it when you need to perform calculations.

```javascript
let age = Number(prompt("Please enter your age:"));

console.log(age);
console.log(typeof age);
```

## 7. Displaying Output with `console.log()`

We use `console.log()` to display information in the browser's developer console.

```javascript
console.log("Hello World");
console.log("I am learning JavaScript");

let age = 20;
console.log(age);
```

To see the output:
1. Open your HTML file in a browser.
2. Right-click on the page.
3. Select **Inspect**.
4. Open the **Console** tab.

In many browsers, `Ctrl + Shift + J` also opens the console.

## 8. Arithmetic Operators

Arithmetic operators perform mathematical calculations.

| Operator | Name | Example | Result |
|---|---|---|---|
| `+` | Addition | `10 + 5` | `15` |
| `-` | Subtraction | `10 - 5` | `5` |
| `*` | Multiplication | `10 * 5` | `50` |
| `/` | Division | `10 / 5` | `2` |
| `%` | Remainder | `10 % 3` | `1` |
| `**` | Exponentiation | `2 ** 3` | `8` |

Example:

```javascript
let num1 = 10;
let num2 = 5;

console.log(num1 + num2);
console.log(num1 - num2);
console.log(num1 * num2);
console.log(num1 / num2);
console.log(num1 % num2);
console.log(2 ** 3);
```

## 9. Assignment Operators

Assignment operators assign a value or update a variable's existing value.

| Operator | Example | Same as |
|---|---|---|
| `=` | `x = 10` | Assign 10 to x |
| `+=` | `x += 5` | `x = x + 5` |
| `-=` | `x -= 5` | `x = x - 5` |
| `*=` | `x *= 5` | `x = x * 5` |
| `/=` | `x /= 5` | `x = x / 5` |
| `%=` | `x %= 5` | `x = x % 5` |

Example:

```javascript
let number = 10;

number += 5;
console.log(number); // 15

number -= 3;
console.log(number); // 12

number *= 2;
console.log(number); // 24

number /= 4;
console.log(number); // 6

number %= 4;
console.log(number); // 2
```

## 10. Practice Examples

### Example 1: Student Information

```javascript
let studentName = "Ali";
let studentAge = 20;
let studentCity = "Karachi";

console.log("Name:", studentName);
console.log("Age:", studentAge);
console.log("City:", studentCity);
```

### Example 2: Add Two Numbers

```javascript
let firstNumber = 15;
let secondNumber = 10;

let total = firstNumber + secondNumber;

console.log("Total:", total);
```

### Example 3: Take Input from a User

```javascript
let firstNumber = Number(prompt("Enter the first number:"));
let secondNumber = Number(prompt("Enter the second number:"));

let result = firstNumber + secondNumber;

console.log("Addition:", result);
```

## Class Practice

Complete these tasks in JavaScript:

1. Create variables for your name, age, and city. Display all three values using `console.log()`.
2. Create one variable using `let` and change its value. Display it before and after changing it.
3. Create three variables using `const` to store your favourite colour, country, and subject.
4. Create one example each of a String, Number, and Boolean.
5. Create a variable without assigning a value. Display it using `console.log()`.
6. Assign `null` to a variable and display it.
7. Use `typeof` to check the data types of at least five values.
8. Use `prompt()` to ask the user for their name, then display a welcome message in the console.
9. Take two numbers from the user and display their addition, subtraction, multiplication, and division.
10. Create a variable with an initial value of `20`. Use `+=`, `-=`, and `*=` to update it. Display the result after each operation.

## Key Takeaways

- Variables store information.
- Use `let` when a value may need to change.
- Use `const` when a variable should not be reassigned.
- Use clear and meaningful variable names.
- JavaScript data types include String, Number, Boolean, `null`, and `undefined`.
- Use `typeof` to check a value's type.
- Use `prompt()` to take input from a user.
- Use `console.log()` to display output in the console.
- Arithmetic operators perform calculations.
- Assignment operators assign or update variable values.

**Keep practising!** Write the examples yourself, change the values, and check the output in your browser console. The best way to learn JavaScript is by writing code and experimenting with it.
