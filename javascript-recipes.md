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

### Module pattern simple implementation

```javascript
var basketModule = (function() {
  var basket = [];  // private field
    return {        // public methods
        addItem: function(values) {
            basket.push(values);
        },
        getItemCount: function() {
            return basket.length;
        },
        getTotal: function() {
           var q = this.getItemCount(),p=0;
            while(q--){
                p+= basket[q].price; 
            }
            return p;
        }
    }
}());
```
("Patterns For Large-Scale JavaScript Application Architecture", Addy Osmani)
