##[Find the smallest integer in the array](https://www.codewars.com/kata/55a2d7ebe362935a210000b2/solutions/javascript)

### Problem:

Given an array of integers your solution should find the smallest integer.

For example:

- Given [34, 15, 88, 2] your solution will return 2

- Given [34, -345, -1, 100] your solution will return -345

You can assume, for the purpose of this kata, that the supplied array will not be empty.

### Solution:

```javascript
class SmallestIntegerFinder {
  findSmallestInt(args) {
    return Math.min(...args)
  }
}
```

```javascript
class SmallestIntegerFinder {
    findSmallestInt(args) {
        Array.min = function(args) {
            return Math.min.apply(Math, args);
        }
      var minimum = Array.min(args);
      return minimum;
    }
}
```

### Similar Kata:

**[Find the smallest](https://www.codewars.com/kata/573992c724fc289553000e95)**

**[Find the integer sequences](https://www.codewars.com/kata/582aad136755daf91a000021)**

**[[JS] Parse integers in array](https://www.codewars.com/kata/535d118ccdbf501816001101)**