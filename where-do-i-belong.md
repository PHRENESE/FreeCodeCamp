http://www.freecodecamp.com/challenges/where-do-i-belong

Return the lowest index at which a value (second argument) should be inserted into an array (first argument) once it has been sorted.

```javascript
function where(arr, num) {
  function order(a, b) {
    return a - b;
  }
  
  var ordered = arr.sort(order);
  
  if (num > ordered[ordered.length - 1]){
    return ordered.length;
  }
  
  for (i=0; i<ordered.length; i++) {
    if (ordered[i] === num) {
      return ordered.indexOf(ordered[i]);
    } else if (ordered[i] < num && ordered[i+1] > num) {
      return ordered.indexOf(ordered[i+1]);
    }
  }
}

where([40, 60], 50);
```
