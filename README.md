# Digx Library

Digx is a simple library that enables you to "dig" values from nested objects using a path. It functions similarly to lodash's `get` method.

## Usage

To use the Digx library, follow these steps:

1. Install Digx by including the library in your project.
2. Import the Digx module into your code.

```javascript
const digx = require('digx');
```

3. Prepare your nested object, `source`, from which you want to extract values.

```javascript
const source = { my: { nested: [1, 2, 3] } };
```

4. Invoke the `digx` function with the `source` object and the desired path as arguments.

```javascript
digx(source, "my.nested[1]"); //=> 2
```

The `digx` function will return the value found at the specified path within the nested object. In the example above, the value `2` is retrieved from the `source` object at the path `"my.nested[1]"`.

Please note that the path syntax follows JavaScript object notation, allowing you to traverse nested objects and arrays using dot notation for objects and square brackets for arrays.

## Conclusion

Digx provides a convenient way to extract values from nested objects by specifying a path. By using Digx in your projects, you can easily access and manipulate data within complex data structures.