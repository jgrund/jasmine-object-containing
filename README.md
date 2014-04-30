jasmine-object-containing
=========================

A simple matcher that wraps jasmine.objectContaining


## Usage
In Node:

```javascript
  var toContainObject = require('jasmine-object-containing').toContainObject;

  beforeEach(function () {
    this.addMatchers(toContainObject);
  });
```

In the browser:

```javascript
  beforeEach(function () {
    this.addMatchers(toContainObject);
  });
```

## Example

```javascript
var obj = {
  foo: function () {},
  bar: 3,
  baz: 10
};

expect(obj).toContainObject({
  foo: jasmine.any(Function),
  bar: 3
});
```
