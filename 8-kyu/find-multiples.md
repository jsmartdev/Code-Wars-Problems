## [Find Multiples of a Number](https://www.codewars.com/kata/58ca658cc0d6401f2700045f)

### Problem: 

In this simple exercise, you will build a program that takes a value, integer , and returns a list of its multiples up to another value, limit . If limit is a multiple of integer, it should be included as well. There will only ever be positive integers passed into the function, not consisting of 0. The limit will always be higher than the base.

For example, if the parameters passed are (2, 6), the function should return [2, 4, 6] as 2, 4, and 6 are the multiples of 2 up to 6.

If you can, try writing it in only one line of code.

### Solutions:

```javascript
function findMultiples(integer, limit) {
  let mults = [];
  for (i = 1; i * integer <= limit; i++) {
    let num = integer * i;
    mults.push(num);
  }
  return mults;  
}
```

```javascript
function findMultiples(int,limit){
  let result = []
  
  for (let i = int; i<=limit ; i+=int)
    result.push(i)
    
  return result
}
```

### Similar Kata:

**[Find factors of a number](https://www.codewars.com/kata/564fa92d1639fbefae00009d)**

**[Find twice of a number's value](https://www.codewars.com/kata/59357d303864834c1a000026)**

**[Find the nth Digit of a Number](https://www.codewars.com/kata/577b9960df78c19bca00007e)**

**[Show multiples of 2 numbers within a range](https://www.codewars.com/kata/583989556754d6f4c700018e)**

**[Find a number increase](https://www.codewars.com/kata/5934ef21b2defb45df000026)**

**[Return the closest number multiple of 10](https://www.codewars.com/kata/58249d08b81f70a2fc0001a4)**