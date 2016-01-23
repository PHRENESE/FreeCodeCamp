http://www.freecodecamp.com/challenges/check-for-palindromes

Return true if the given string is a palindrome. Otherwise, return false.

```javascript
function palindrome(str) {
  str = str.toLowerCase().replace(/\W|_/g, '');
  var rev = str.split("").reverse().join("");
  
  if (str != rev){
    return false;
  } else {
    return true;
  }
}

palindrome("eye");
```
