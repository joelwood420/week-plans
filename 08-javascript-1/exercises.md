# Week 8 Exercises


**NOTE:** Whenever these exercises talk about 'user input', you'll have to use a
variable in your code and assign it a value. We'll find out soon how to actually
ask the user for input.

## 1. Variable Naming Brainstorm

How would you name variables that hold the following information? For every bullet point
**give one good and one bad example**.

1. the current outside temperature
2. your favorite Pizza topping
3. the number of characters in a string

## 2. Hello, world!

Recreate the hello world example from the slides.

- One HTML page with a `<script>` tag in the body.
- One HTML page that links an external file `exercise.js` in its `<head>`

Either script should just print "Hello, world!" to the console.

## 3. Strings

Find out about the "string concatenation operator +" in Javascript.

1. Demonstrate concatenating a string with a string. Print the output to the console if possible.
2. Demonstrate concatenating a string with a number. Print the output to the console if possible.
3. Demonstrate concatenating a number with a string. Print the output to the console if possible.

Find out about "string interpolation" in Javascript.

1. Demonstrate string interpolation. Interpolate a string with a variable that stores a number.
   Print the output to the console if possible.

---

## 4. Simple Grading System

Write a program that takes a student's test score (e.g., 85) and prints out
their grade (e.g., "A" for scores 90 and above, "B" for 80-89, etc.). Anything
below score 50 is an "F".

## 5. Simple Password Checker

Write a program that checks if a password (stored in `password`) matches a predefined password
(stored in `expectedPassword`, could be `thisismypassword`) and displays a message like 
"Access Granted" or "Access Denied."

## 6. Weather Outfit Selector

Create a script that suggests what to wear based on the weather. You input a temperature,
and the script tells you what to wear.

For example, if it's cold (under 15 degrees), suggest wearing a jacket.
If it's warm, but not hot (between 15 and 25 degrees), suggest a jumper.
if it's hot (above 25 degrees), suggest shorts.

## 7. How to ask the user for input

Find out how to use the `prompt()` function in JavaScript. Apply your learning to any of the three
previous activities.

## 8. Time or Date Output

Write a program that asks the user whether they want to see the time or the
date. If they type "time", then show them the time on the console. If they type
"date", show them the date on the console.

You can use the following snippets to get date and time as a string:
```js
const date = new Date().toDateString();
const time = new Date().toTimeString();
```

---

## 9. Math Wizard
Create a function for each of the following operations: addition, subtraction, multiplication, and division.
The functions should take two numbers as parameters and return the result of the operation.

Example:
```js
function add(num1, num2) {
  return num1 + num2;
}
```

## 10. Greeting Generator
Write a function called greet that takes a person's name as a parameter and returns a personalized greeting, like "Hello, [name]!".
Then log the output.

Sample code without the function itself;
```
let greeting = greet("Hortensia");
console.log(greeting);
```

## 11. Weight Converter
Your best friend from England, Sir Vortex Throckmorton, is visiting. You're cooking a meal together.
As he uses different units than you (pounds instead of kilograms), you write a small program to help
you communicate.

Write two functions: one to convert imperial pounds to kilograms and another to convert kilograms to imperial pounds.
Each function should take one parameter (the weight) and return the converted value.

The formula for that is: `kilograms = pounds / 2.2` and `pounds = kilograms * 2.2`

Example call:
```
console.log(kilosToPounds(10)); // should log `22`
```

Convert all these values:
12 pounds
14 pounds
0 pounds
-5 pounds
1 kilo
0.512 kilos
2342324323 kilos

## 12. Calculator
Take your first activity, the math wizard, and re-write it to use only one function:

```
function calculate(num1, num2, operator) {

}
```

## 13. Project: Order Management System
You are building a simple order management system for a small online store. The system needs to handle different types of products and calculate the final price based on specific conditions.

We'll build a frontend for this project in the coming weeks. For now, we'll focus on JavaScript.

Create a function `calculatePrice`

The function should take three arguments: `productType`, `quantity`, and `isMember`.

- `productType` will be a string representing the type of product (e.g., "electronics", "clothing", "grocery").
- `quantity` will be an integer representing the number of items.
- `isMember` will be a boolean indicating whether the customer is a store member (true/false).

Set up base prices:
- Electronics: $100 per item
- Clothing: $50 per item
- Grocery: $20 per item

Apply discounts and conditions:
- If the customer is a member, apply a 10% discount on the total price.
- If the customer buys more than 5 items of any product type, apply an additional 5% discount on the total price.
- Ensure that the discounts are applied in the correct order (first membership discount, then bulk discount).

Return the final price: The function should return the final price as a number.

### Example Outputs

- `calculatePrice("electronics", 3, true)` should return `270` (300 - 10% discount).
- `calculatePrice("clothing", 6, false)` should return `285` (300 - 5% discount).
- `calculatePrice("grocery", 7, true)` should return `119` (140 - 10% discount - 5% discount).

### Bonus Challenge

Modify the function to add a special promotion: if the total price after discounts exceeds $500, apply a $50 discount.

