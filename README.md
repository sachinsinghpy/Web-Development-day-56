# Web-Development-day-56
JavaScript conditional statement
f else conditionals
The "if" statement in JavaScript is used to execute a block of code if a certain condition is met. The "else" clause is used to execute a block of code if the condition is not met.

Here is the basic syntax for an "if" statement:

if (condition) {
  // code to be executed if condition is true
}

Here is the syntax for an "if" statement with an "else" clause:

if (condition) {
  // code to be executed if condition is true
} else {
  // code to be executed if condition is false
}

The condition is a boolean expression that evaluates to either true or false. If the condition is true, the code in the "if" block is executed. If the condition is false, the code in the "else" block is executed (if present).

For example:

let x = 10;
if (x > 5) {
  console.log("x is greater than 5");
} else {
  console.log("x is not greater than 5");
}

In this example, the condition x > 5 is true, so the code in the "if" block is executed and the message "x is greater than 5" is printed to the console.

If else ladder
The "if-else ladder" is a control structure in JavaScript that allows you to execute a different block of code depending on multiple conditions. It is called a ladder because it consists of multiple "if" and "else" statements arranged in a ladder-like fashion.

Here is the syntax for an "if-else ladder":

if (condition1) {
  // code to be executed if condition1 is true
} else if (condition2) {
  // code to be executed if condition1 is false and condition2 is true
} else if (condition3) {
  // code to be executed if condition1 and condition2 are false and condition3 is true
} ...
else {
  // code to be executed if all conditions are false
}

In this structure, each "if" statement is followed by an optional "else" statement. If the first "if" condition is true, the code in the corresponding block is executed and the rest of the ladder is skipped. If the first "if" condition is false, the second "if" condition is evaluated, and so on. If none of the conditions are true, the code in the "else" block is executed.

For example:

let x = 10;
if (x > 15) {
  console.log("x is greater than 15");
} else if (x > 10) {
  console.log("x is greater than 10 but less than or equal to 15");
} else if (x > 5) {
  console.log("x is greater than 5 but less than or equal to 10");
} else {
  console.log("x is less than or equal to 5");
}

In this example, the first "if" condition x > 15 is false, so the second "if" condition x > 10 is evaluated. This condition is also false, so the third "if" condition x > 5 is evaluated. This condition is true, so the code in the corresponding block is executed and the message "x is greater than 5 but less than or equal to 10" is printed to the console.

The "if-else ladder" is a useful control structure for executing different blocks of code based on multiple conditions. It can help you write more concise and maintainable code in JavaScript.


Ternary Operator
The ternary operator is a shorthand way to write an if-else statement in JavaScript. It takes the form of condition ? value1 : value2, where condition is a boolean expression, and value1 and value2 are expressions of any type. If condition is true, the ternary operator returns value1; if condition is false, it returns value2.

Here's an example of how you can use the ternary operator to assign a value to a variable based on a condition:

let x = 10;
let y = 20;
let max;
 
max = (x > y) ? x : y;
 
console.log(max); // Outputs: 20

In this example, the ternary operator checks whether x is greater than y. If it is, max is assigned the value of x; otherwise, it is assigned the value of y.

The ternary operator can be a useful and concise way to write simple if-else statements, but it can become difficult to read and understand when used for more complex statements or nested inside other expressions. In these cases, it may be better to use a regular if-else statement instead.
