Given n, take the sum of the digits of n. 
If that value has more than one digit, continue reducing in this way until a single-digit number is produced. 
The input will be a non-negative integer.

```js
function digital_root(n) {
  while(n.toString().length>=2){
    let arr = n.toString().split('');
    n = arr.reduce(function(previousValue,currentValue){
        return parseInt(previousValue) + parseInt(currentValue);
      })
  }
   return n;
}
```
