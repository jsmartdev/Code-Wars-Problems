##[Even or Odd](https://www.codewars.com/kat53da3dbb4a5168369a0000fesolutions/javascript)

### Problem:

Create a function that takes an integer as an argument and returns "Even" for even numbers or "Odd" for odd numbers.

### Solutions:

```javascript
function even_or_odd(number) {
  if (number % 2 === 0) {
    return "Even";
  }
  else {
    return "Odd";
  }
}
```

```javascript
function even_or_odd(number) {
  return number % 2 ? "Odd" : "Even"
}
```

### Similar Kata:

**[Odd or Even?](https://www.codewars.com/kata/5949481f86420f59480000e7)**

**[Even or Odd - Which is Greater?](https://www.codewars.com/kata/57f7b8271e3d9283300000b4)**