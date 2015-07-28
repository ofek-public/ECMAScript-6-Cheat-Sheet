# ECMAScript-6-Cheat-Sheet
Summary of ECMAScript 6 features

## arrow functions
```javascript
    x => x + 1
    (x, y) => x + y
    x => {return x + 1}
```

## array destructuring
```javascript
    var [x, , y] = [1,2,3]; // x === 1, y === 3
    var [x] = []; // x === undefined
    var [x = 1] = []; // x === 1 (default value)
    var [x, y, z] = "xyz"; // x === "x", y === "y", z === undefined
```

## object destructuring
```javascript
    var {x, a:y: z} = {x: 1, y: 2}; // x === 1, a === 2, z === undefined
```

## `Number` properties
```javascript
    Number.isFinite
    Number.isInteger
    Number.isSafeInteger
    Number.isNaN
    Number.EPSILON // 2.220446049250313e-16
    Number.MIN_SAFE_INTEGER // -9007199254740991
    Number.MAX_SAFE_INTEGER // 9007199254740991
```

## `Math` methods
```javascript
    Math.clz32
    Math.imulc
    Math.sign
    Math.log10
    Math.log2
    Math.log1p
    Math.expm1
    Math.cosh
    Math.sinh
    Math.tanh
    Math.acosh
    Math.asinh
    Math.atanh
    Math.trunc
    Math.fround
    Math.cbrt
    Math.hypot
```
