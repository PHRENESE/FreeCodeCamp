http://www.freecodecamp.com/challenges/find-the-longest-word-in-a-string

Return the length of the longest word in the provided sentence.

```javascript
function findLongestWord(str) {
  var words = str.split(" ");
  var longest = 0;
  for(i=0;i<words.length;i++){
    var place = words[i].length;
    if(place > longest){
      longest = place;
    }
  }
  return longest;
}

findLongestWord('The quick brown fox jumped over the lazy dog');
```
