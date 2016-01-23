http://www.freecodecamp.com/challenges/mutations

Return true if the string in the first element of the array contains all of the letters of the string in the second element of the array.

```javascript
function mutation(arr) {
  var source = arr[0].toLowerCase().split('');
  var keys = arr[1].toLowerCase().split('');
  for(i = 0; i < keys.length; i++){
    if (source.indexOf(keys[i]) < 0)
      return false;
    }
    return true;
}

mutation(["hello", "hey"]);
```

This was my first wrong solution:
```javascript
function mutation(arr) {
  var One = arr[0].toLowerCase().split('').sort().join('') ;
  var Two = arr[1].toLowerCase().split('').sort().join('') ;
  if(One.indexOf(Two) !== -1){
    return true;
  } else {
    return false;
  }
}

mutation(["hello", "hey"]);
```
