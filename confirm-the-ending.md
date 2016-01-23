http://www.freecodecamp.com/challenges/confirm-the-ending

Check if a string (first argument) ends with the given target string (second argument).

```javascript
function end(str, target) {
  if (str.substr(-target.length) === target) {
    return true;
  } else {
    return false;
  }
}

end("Bastian", "n");
```
