http://www.freecodecamp.com/challenges/return-largest-numbers-in-arrays

Return an array consisting of the largest number from each provided sub-array.
For simplicity, the provided array will contain exactly 4 sub-arrays.

```javascript
function largestOfFour(arr) {
  // You can do this!
  var biggest = [];
  for(i=0;i<arr.length;i++){
    var temp = 0;
    for(j=0;j<arr[i].length;j++){
      if(arr[i][j] > temp ){
        temp = arr[i][j];
      }
      biggest[i] = temp;
    }
  }
  return biggest;
}

largestOfFour([[4, 5, 1, 3], [13, 27, 18, 26], [32, 35, 37, 39], [1000, 1001, 857, 1]]);
```
