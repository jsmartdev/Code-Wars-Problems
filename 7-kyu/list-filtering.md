## [List Filtering](https://www.codewars.com/kata/53dbd5315a3c69eed20002dd)

### Problem:

In this kata you will create a function that takes a list of non-negative integers and strings and returns a new list with the strings filtered out.

**Example**

```
filter_list([1,2,'a','b']) == [1,2]
filter_list([1,'a','b',0,15]) == [1,0,15]
filter_list([1,2,'aasf','1','123',123]) == [1,2,123]
```

### Solutions:

```javascript
function filter_list(l) {
  // Return a new array with the strings filtered out
  let noStrings = [];
  for (i = 0; i < l.length; i++) {
    let index = l[i];
    if (typeof index != 'string') {
      noStrings.push(index);
    }
  }
  return noStrings;
}
```

```javascript
function filter_list(l) {
  return l.filter(function(v) {return typeof v == 'number'})
}
```

### Similar Kata:

**[Fun with lists: filter](https://www.codewars.com/kata/582041237df353e01d000084)**

**[Number Shortening Filter](https://www.codewars.com/kata/56b4af8ac6167012ec00006f)**

**[Javascript filter - 3](https://www.codewars.com/kata/525f0459fb9570f9ff00005d)**

**[Filter Coffee](https://www.codewars.com/kata/56069d0c4af7f633910000d3)**

**[Filter out for good!](https://www.codewars.com/kata/56035d75426e197c3e0000a2)**

