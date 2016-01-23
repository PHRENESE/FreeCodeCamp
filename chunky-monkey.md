http://www.freecodecamp.com/challenges/chunky-monkey

Write a function that splits an array (first argument) into groups the length of size (second argument) and returns them as a multidimensional array.

Bunch of variations, I was trying to make the size increment the most readable.

```javascript
function chunk(arr, size) {
  var newArr = [];
  for (var i = 0; i < arr.length; i += size) {
    newArr.push(arr.slice(i, i + size));
  }
  return newArr;
}

chunk(["a", "b", "c", "d"], 2, "");
```

```javascript
function chunk(arr, size) {
  var multi = [];
  i = 0;
  while (i < arr.length) {
		multi.push(arr.slice(i, i+size));
    i = i+size;
  }
  console.log(multi);
}

chunk(["a", "b", "c", "d"], 1);
```

```javascript
function chunk(arr, size) {
  var multi = [];
  for (i = 0; i < arr.length; i+=size){
    multi.push(arr.slice(i, i+size));
  }
  return multi;
}

chunk(["a", "b", "c", "d"], 2);
```
