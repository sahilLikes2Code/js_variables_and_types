## If Statement

1.  🎖Make a simple calculator with these functions. Using prompt, type conversion, if else statement. Use prompt to take the input from user i.e two numbers and an operation (Add, Sub, Mul, Div).

⛑ Rule
_ [ ] While substracting and dividing keep in mind the number one should be greater then number two. If not show alert saying `Number Two is larger then Number one`.
⚡️ Operations
````js
_ [ ] Add

_ [ ] Sub

_ [ ] Mul

_ [ ] Div


function Add (x, y) {
  var result =  x + y;
  alert(`${x} +  ${y} is equal to ${result}`);
}

function Sub (x, y) {
if (x > y) {
  var result =  x - y;
  alert(`${x} - ${y} is equal to ${result}`);
}
}

function Mul (x, y) {
  var result = x * y;
  alert(`${x} * ${y} is equal to ${result}`);
}

function Div (x, y) {
if (x > y) {
  var result = x / y;
  alert(`${x} / ${y} is equal to ${result}`);
} else {
  alert('Number two is larger than Number one. Make valid entries');
}
}

const x = Number(prompt('Enter the first number', ''));
const y = Number(prompt('Enter the second number', ''));
let operation = prompt('Enter the operation: Add, Sub, Mul or Div', '');

if (operation == 'Mul' || operation == 'Sub' || operation == 'Add' || operation == 'Div' ) {
    if (operation == 'Add') {
    Add (x, y);
  } else if (operation == 'Sub') {
    Sub (x, y);
  } else if (operation == 'Div') {
    Div(x, y);
  } else if(operation == 'Mul') {
    Mul(x, y);
  }
} else {
  alert('Enter a valid Operator');
}

// }
````

2. 🎖Write an if else statement which checks if the status is single `console.log` the message `John is single` or else `John is married`
```js
var firstName = 'John';
var status = 'single';
// Your code goes here
if (status == "single") {
  console.log("John is single");
} else {
  console.log("John is married");
}
````

3. 🎖Write a JavaScript program that takes two `integers` from user (using prompt) and alerts the larger number.

// ```js
// your code goes here

var numberOne = prompt("Enter a number", "");
var numberTwo = prompt("Enter another number", "");
if (numberOne > numberTwo) {
  prompt(`${numberOne} is greater out of the two numbers entered`);
} else {
  prompt(`${numberTwo} is greater out of the two numbers entered`);
}
```

4. 🎖Write a JavaScript conditional statement to find the sign (+, -) of product of three numbers. Take those three numbers from user using `prompt`. Display an alert box with the specified sign.

```js
// Your code goes here
var firstNumber = prompt("Enter the first number");
var secondNumber = prompt("Enter the second number");
var thirdNumber = prompt("Enter the third number");
var productOfThreeNumbers = firstNumber * secondNumber * thirdNumber;
if (productOfThreeNumbers > 0)
  alert("The sum of three numbers is '+' positive");
else {
  alert("The sum of three numbers is '-' negative");
}
```

## Switch Statement

1. 🎖Using switch statement do the following

Take a number value from user and alert the message if it matches the conditions.

- [ ] ONE, if `number` is equal to 1.
- [ ] TWO, if `number` is equal to 2.
- [ ] THREE, if `number` is equal to 3.
- [ ] FOUR, if `number` is equal to 4.
- [ ] FIVE, if `number` is equal to 5.
- [ ] SIX, if `number` is equal to 6.
- [ ] SEVEN, if `number` is equal to 7.
- [ ] EIGHT, if `number` is equal to 8.
- [ ] NINE, if `number` is equal to 9.
- [ ] PLEASE TRY AGAIN, if is none of the above.

```js
// Your code goes here
var a = Number(prompt("Enter a number from 0 to 9"));

switch (a) {
  case 1:
    alert("ONE");
    break;
  case 2:
    alert("Two");
    break;
  case 3:
    alert("Three");
    break;
  case 4:
    alert("Four");
    break;
  case 5:
    alert("Five");
    break;
  case 6:
    alert("Six");
    break;
  case 7:
    alert("Seven");
    break;
  case 8:
    alert("Eight");
    break;
  case 9:
    alert("Nine");
    break;
  default:
    alert("Please try again");
}
```

2. 🎖Using switch statement do the following

Take the value of `marks` (0-100) from user using `prompt` and `alert` the message (Your Grade is AA) as giver below.

- [ ] `AA` if `marks` is greater than 90.
- [ ] `AB` if `marks` is greater than 80 and less than or equal to 90
- [ ] `BB` if `marks` is greater than 70 and less than or equal to 80
- [ ] `BC` if `marks` is greater than 60 and less than or equal to 70
- [ ] `CC` if `marks` is greater than 50 and less than or equal to 60
- [ ] `CD` if `marks` is greater than 40 and less than or equal to 50
- [ ] `DD` if `marks` is greater than 30 and less than or equal to 40
- [ ] `FF` if `marks` is less than or equal to 30

```js
// Your code goes here

var marks = Number(
  prompt("Enter your score and i will translate it to grades")
);

switch (true) {
  case marks > 90:
    alert("Your grade is AA");
    break;
  case marks > 80 && marks <= 90:
    alert("Your grade is AB");
    break;
  case marks > 70 && marks <= 80:
    alert("Your grade is BB");
    break;
  case marks > 60 && marks <= 70:
    alert("Your grade is BC");
    break;
  case marks > 50 && marks <= 60:
    alert("Your grade is CC");
    break;
  case marks > 40 && marks <= 50:
    alert("Your grade is CD");
    break;
  case marks > 30 && marks <= 40:
    alert("Your grade is DD");
    break;
  case marks >= 30:
    alert("Your grade is FF");
    break;
  default:
    alert("Please enter a number greater than 30 or equal to 100");
}
```
