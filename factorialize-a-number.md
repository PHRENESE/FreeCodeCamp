http://www.freecodecamp.com/challenges/factorialize-a-number

As I've read multiple times, recursion while being more elegant is most of the times slower than a regular loop.
I tested this with jsperf on a simple factorial function. Here is the [JSPerf](http://jsperf.com/factorial-recursive) link if you want to test on your own machine.

Recursion:
```javascript
function factorialize(num) {
  if (num <= 0) {
    return 1;
  }
  return num * (factorialize(num-1));
}

factorialize(5);
```
Result: 30,406,485 Ops/sec
±0.51%
59% slower

Basic for loop: 
```javascript
function factorialize(num) {
 var result = 1;
  for (i = 1; i <= num; i++) {
 result = result * i;
  }
return result;
}

factorialize(5);
```
Result:
73,615,404 Ops/sec
±0.47%
fastest
