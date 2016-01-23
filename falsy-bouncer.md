http://www.freecodecamp.com/challenges/falsy-bouncer

Remove all falsy values from an array.

Falsy values in javascript are false, null, 0, "", undefined, and NaN.

```javascript
function bouncer(arr) {
  var truthy = arr.filter(Boolean);
  return truthy;
}

bouncer([7, "ate", "", false, 9]);
// -> [7, "ate", 9]
```
