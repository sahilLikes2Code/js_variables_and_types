1. In code below "Mark" is a string.  What is name?
```js
var name = "Mark";
```
// name is variable with identifier "Mark"

2. Find the error if any
```js
  var product cost = 3.45;
```
// The variable identifier is incorrectly defined as JS does not support gap/space. Alternatively, the developer can make use of the camel casing writing convention. Following which the identitfier will look like "productCost" 

3. Write `Right or Wrong` next to the code below.

```js
  "Hello World" : Right
  'Hello World" : Wrong
  "Hello World' : Wrong
  'Hello World' : Right
```


## Write `VALID` and `INVALID` infront of the variable name defined below
```js
var man; VALID
var 1girl; INVALID
var woman3; VALID
var -girl; INVALID
var blackDog; VALID
var 42; VALID
var $42; VALID
var userName; VALID
var x, y, z; VALID
var x = 5, y = 6, z = 7; VALID
var x = 5 + 10 + 2; VALID
```

## Basic Operations

Mathematical Operations:

Solve this using mathematical operations. (+, -, *, / , etc)

```js
var amount = 2080;
// Define a new variable and store the value that is 80 less then the value of amount.
var iSubtract80From_amount = amount - 80;
// Define a new variable and store the value that is 200 more then the value of amount.
var iAdd200To_amount = amount + 200;
// Define a new variable and store the value that is 4 times the value of amount.
var iMultiplyThe_amountwith4 = amount*4;
// Define a new variable and store the reminder when the value of amount is  divided by 21.
var iGiveOutTheRemainderWhenAmountIsDividedWith21 = 2080 % 21;
```

Logical Operation:

Solve this using logical operations. (<, >, &&, ||)

```js
var johnAge = 45;
var markAge = 35;

// Check who is older either John or Mark
if (johnAge < markAge) {
  console.log('Mark is older');
} else {
  console.log('John is older');
}
// Check who is younger
if (johnAge < markAge) {
  console.log('John is Younger');
} else {
  console.log('Mark is Younger');
}

// Check if their age is equal
if (johnAge ===  markAge) {
  console.log('Both of them are the same age');
} else {
  console.log('Their age is not same');
}
// Create a new variable and assign the age of john to new variable.
var john = johnAge;
// Create a new variable and assign the age of mark to new variable.
var mark = markAge;
// Check if john is equal to or greater then mark.
if (john >= mark) {
  console.log ("John is less than or equal to mark");
} else {
  console.log("Mark is greater than John");
}
// Check if john is less then or equal to mark.
if (john <= mark) {
  console.log("John is less than or equal to mark");
} else {
  console.log("John is greater than Mark");
}
// Calculate the average age of john and mark and assign to a new variable.
var combinedAge = johnAge + markAge;
var averageAge = combinedAge/2;
```