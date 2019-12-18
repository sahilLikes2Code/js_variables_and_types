1. 🎖 Write a program to calculate the total price of your phone purchase. With these conditions
 * [ ] You will keep purchasing phones (hint: loop!) until you run out of bank balance.
 * [ ] You'll also buy accessories for each phone as long as your purchase amount is below your spending threshold.
 * [ ] After you've calculated your purchase amount, add in the tax, then print out the calculated purchase amount, properly formatted.
 * [ ] Finally, check the amount against your bank account balance to see if you can afford it or not.
 * [ ] Write a function called calculateTax which takes an argument 'amount' and calculates the tax you need to pay.
 * [ ] Write a function named formatAmount which returns you amount in this format '$ 132.45' make the decimal fixed to 2 places.
```js
const SPENDING_THRESHOLD = 200;
const TAX_RATE = 0.08;
const PHONE_PRICE = 99.99;
const ACCESSORY_PRICE = 9.99;

var bank_balance = 303.91;
var amount = 0;
// your code goes here


var totalCostOfPhoneAndAccessories = PHONE_PRICE + ACCESSORY_PRICE;
var totalCostOfPhoneAndAccessoriesWithTax = (1 + TAX_RATE) * totalCostOfPhoneAndAccessories;
console.log(totalCostOfPhoneAndAccessoriesWithTax);

if (totalCostOfPhoneAndAccessoriesWithTax <= bank_balance) {
    console.log("Yay! You can afford the phone and accessories");
} else {
    console.log("You don't have enough money to buy this smartphone");
}

function calculateTax (amount) {
    var tax = (amount * TAX_RATE) / 100;
    return tax;
}
calculateTax(100);

function formatAmount () {
    roundedNumber = totalCostOfPhoneAndAccessoriesWithTax.toFixed(2);
    return(`The total amount is ${roundedNumber}`);
}


var remainingBalance = SPENDING_THRESHOLD - totalCostOfPhoneAndAccessoriesWithTax;

while (remainingBalance > totalCostOfPhoneAndAccessoriesWithTax) {
  console.log("You can atleast buy one smartphone");
}

```
 ⛑ Answer of the above will `$334.76`.

2. 🎖 Write a for loop that will iterate from 0 to 20. For each iteration, it will check if the current number is even or odd, and report that to the screen using `alert` (e.g. "2 is even").
```js
// your code goes here
for (i = 0; i <= 20; i++) {
    var remainder = i % 2;
    if (remainder == 0 ) {
        alert(`${i} is an even number`);
    } else {
         alert(`${i} is an odd number`);
    }
}


3. 🎖Write a for loop that will iterate from 0 to 10. For each iteration of the for loop, it will multiply the number by 9 and log the result in console (e.g. "2 * 9 = 18").
// your code goes here
for (i = 0; i <= 10; i++) {
    var multiplyWith10 = i * 9;
    console.log(`${i} * 9 = ${multiplyWith10}`);
}

4. 🎖Use a nested for loop to show the tables for every multiplier from 1 to 10 (100 results total).
(e.g.
"1 * 1 = 1"
"1 * 2 = 2"
"1 * 3 = 3"
"1 * 4 = 4"
.... for all 100 results)
// your code goes here
for (i = 1; i <= 10; i++) {
    for (j = 1; j <= 10; j++) {
        var totalOfTwoNumbers = i * j;
        console.log(`${i} * ${j} = ${totalOfTwoNumbers}`)
    }
}

5. 🎖Show the following output using one loop.
// -------------------------------------------------------------------
// 1, 2, 3, 4, 5
// 6, 7, 8, 9, 10

// Your code goes here
var s = "";
for (i = 1; i <= 5; i++) {

    s+= (`${i}, `);
}
console.log(s);
// -------------------------------------------------------------------

6. 🎖Use a while loop to add up the numbers 1 to 20.
// js
// Your code goes here

var sum  = 0;
var number = 1;

while (number <= 20) {
    sum = sum + number;
    number++;
}
console.log("Sum = " + sum);


7. 🎖Use a while loop to print out the even number from 1 to 20. (You'll need Modulus for this. And an IF Statement.)
// js
// Your code goes here

var container = 0;
var num = 1;

while (num <= 20) {
    var remainder = num % 2;
    if (remainder == 0) {
        console.log (num);
    }
    num++;
}



