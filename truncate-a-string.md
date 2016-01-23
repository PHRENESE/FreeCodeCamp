http://www.freecodecamp.com/challenges/truncate-a-string

Truncate a string (first argument) if it is longer than the given maximum string length (second argument).
Return the truncated string with a "..." ending.

Note that the three dots at the end add to the string length.

If the num is less than or equal to 3, then the length of the three dots is not added to the string length.

Low brow literal solution:
```javascript
function truncate(str, num) {
  if (num <= 3) {
    return str.slice(0,num) + "...";
  }
  if (str.length > num) {
    return str.slice(0,num-3) + "...";
  }
  if (num >= str.length) {
    return str;
  }
}

truncate("A-tisket a-tasket A green and yellow basket", 2);
```

More concise:
```javascript
function truncate(str, num) {
  var i = 0;
  if (num >= 3){
    i=3;
  }

  if (str.length> num) {
    str= str.slice(0,num-i)+"...";}
  console.log(str);
} 

truncate("A-tisket a-tasket A green and yellow basket", 1);
```
