# -Narcissistic-Numbers

## Problem

A Narcissistic Number is a number of length n in which the sum of its digits to the power of n is equal to the original number. If this seems confusing, refer to the example below.

Ex: 153, where n = 3 (number of digits in 153)
13 + 53 + 33 = 153

Write a method is_narcissistic(i) (in Haskell: isNarcissistic :: Integer -> Bool) which returns whether or not i is a Narcissistic Number.

## Solution

```javascript
const isNarcissistic = (n) => {
var nums = 0;
var numbers = String(n);
 for(let i of numbers) {
   nums += Number(i) ** numbers.length;
 }
  return  nums === n;
} 

console.log(isNarcissistic(153));

true
```
