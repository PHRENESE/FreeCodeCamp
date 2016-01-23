http://www.freecodecamp.com/challenges/repeat-a-string-repeat-a-string

Repeat a given string (first argument) n times (second argument).
Return an empty string if n is a negative number.

```javascript
function repeat(str, num) {
  var newstr = [];
  for (var i = 0; i < num; i++) {
    newstr.push(str);
  }
  return newstr.join('');
}

repeat("abc", -1);
```
