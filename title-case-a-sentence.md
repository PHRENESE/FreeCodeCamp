http://www.freecodecamp.com/challenges/title-case-a-sentence

Return the provided string with the first letter of each word capitalized. Make sure the rest of the word is in lower case.

For the purpose of this exercise, you should also capitalize connecting words like "the" and "of".

```javascript
function titleCase(str) {
  var words = str.toLowerCase().split(" ");
  for (i = 0; i < words.length; i++) {
    words[i] = words[i].charAt(0).toUpperCase() + words[i].substring(1);
  }
  return words.join(" ");
}

titleCase("I'm a little tea pot");
```
