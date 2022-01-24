Write a function that takes an (unsigned) integer as input, and returns the number of bits that are equal to one in the binary representation of that number.
Example: The binary representation of 1234 is 10011010010, so the function should return 5 in this case.

```js
var countBits = function(n) {
   //convert n to binary form and then to an array
   const arr = (n).toString(2).split('');
   
   bits = arr.reduce(function(previousValue, currentValue){
    previousValue *=1;
    currentValue *=1;
    
    return previousValue + currentValue
   })
   return bits;
};
```
