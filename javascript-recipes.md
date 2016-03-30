### How to loop throught array removing its elements

Simplest way is to iterate an array in reverse to avoid extra index decrement

```javascript
var i = array.length;
while (i--) {
  // do something;
  array.splice(i, 1);
}
```
[Source](http://stackoverflow.com/questions/9882284/looping-through-array-and-removing-items-without-breaking-for-loop)
