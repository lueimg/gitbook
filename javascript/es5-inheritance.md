# es5 inheritance

```javascript
var Shape = function() {}
Shape.prototy.getName = function() {
    // ...
}

var Rectangle = function() {
    Shape.call(this);
}

Rectangle.prototype = Object.Create(Shape.prototype);
Rectangle.prototype.constructor = Rectangle;

```

