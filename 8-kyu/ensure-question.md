##[Ensure question](https://www.codewars.com/kata/5866fc43395d9138a7000006/javascript)

### Problem:

Given a string, write a function that returns the string with a question mark ("?") appends to the end, unless the original string ends with a question mark, in which case, returns the original string.

For example (Input --> Output)

```
"Yes" --> "Yes?" 
"No?" --> "No?"
```

### Solutions: 

```javascript
function ensureQuestion(s) {
  let a = s.length - 1;
  if (s[a] === "?") {
    return s;
  }
  else {
    let b = "?";
    s += b;
    return s;
  }
}
```

```javascript
const ensureQuestion = s => s.endsWith('?') ? s : s+'?'
```

### Similar Kata:

**[Feynman's square question](https://www.codewars.com/kata/551186edce486caa61000f5c)**

**[Interview Question (easy)](https://www.codewars.com/kata/5b358a1e228d316283001892)**