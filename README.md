jasmine-object-containing
=========================

A simple matcher that wraps jasmine.objectContaining


## Usage

Make sure the jasmine-object-containing.js file is executed early in your tests, it uses `beforeEach` to register the matcher.

## Example

```javascript
var obj =  {
  foo: function () {},
  bar: 3,
  baz: 10
};

expect(obj).toContainObject({
  foo: jasmine.any(Function),
  bar: 3
});
```
