##[Sum of positive](https://www.codewars.com/kata/5715eaedb436cf5606000381)

### Problem:

You get an array of numbers, return the sum of all of the positives ones.

Example [1,-4,7,12] => 1 + 7 + 12 = 20

Note: if there is nothing to sum, the sum is default to 0.

### Solutions: 

```javascript
function positiveSum(arr) {
    var total = 0;
    // setup loop to go through array of given length    
    for (i = 0; i < arr.length; i++) { 
        // if arr[i] is greater than zero     
        if (arr[i] > 0) { 
            // add arr[i] to total                    
            total += arr[i];                  
        }
    }
    // return total
    return total;
}
```

```javascript
function positiveSum(arr) {
   return arr.reduce((a,b)=> a + (b > 0 ? b : 0),0);
}
```