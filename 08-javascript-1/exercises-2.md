## JS, Exercises

Write code to:

### Exercise 1 (3min)

Output the value "First one's always the hardest" to the developer console.

console.log("First one's always the hardest");

### Exercise 2 (3min)

Type out the following symbols:

1. a pair of parentheses ()
2. a pair of square brackets []
3. a colon :
4. a semi-colon ;
5. a pair of braces {}

### Exercise 3 (3min)

Which digits are used

1. in hexadecimal notation? 0-9, A-F
2. in binary notation? 0, 1


### Exercise 4 (3min)

Write a script tag that includes a JavaScript file named "review.js" into HTML

<script src="review.js"></script>

### Exercise 5 (3min)

Use `node` on your terminal to evaluate the following expression:

```js
2 ** (2 + "1") / 4 / 4 / 4 / (4 / 4) / 10 ** 6;
```


What is the result? 0.032768

### Exercise 6 (3min)

Declare an immutable variable named `gymbro` and initialize it with any boolean
value.

let gymBro = true;

### Exercise 7 (3min)

Build a comparison between a variable named `legDay` and the number 90. The
comparison should check whether they are equal in type and value.

let legDay = 90;
console.log(legDay === 90);

### Exercise 8 (3min)

Translate this string concatenation into a string interpolation:

```js
let personOrBarnacle = "Patrick";
let greeting = "Hello ";
let result = greeting + "this is " + personOrBarnacle + "!?";

let result = `${greeting}this is ${personOrBarnacle}!?`;
```

### Exercise 9 (3min)

Write an `if`-statement so that:

- when health is equal or greater to 10 but smaller than 50, it should print "not terrible"
- when health is equal or less than 0, it should print "terrible"
- when health is equal or greater to 50, it should print "optimal"

Start like this:

```js
let health = 50;

if (health >= 10 && health < 50) {
    console.log("not terrible");
} else if (health <= 0) {
    console.log("terrible");
} else if (health >= 50) {
    console.log("optimal");
}
```

### Exercise 10 (3min)

Write a while-loop that adds 1 to a variable until the variable reaches 10. Print the variable every loop.

Start like this:

```js
let variable = 0;

while (variable < 100) {
    variable++;

    let output = "";
    if (variable % 3== 0) {
     output += 'pop'
    } if (variable % 5 == 0){
     output += 'buzz'
    }
    
     else {
        output = variable
     } 

     console.log(output);
   
}

