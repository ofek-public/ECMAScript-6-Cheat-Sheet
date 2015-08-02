# ECMAScript 6 Cheat Sheet

### Arrow functions
```javascript
    x => x + 1                          // similar to function(x) {return x + 1;}
    (x, y) => x + y                     // similar to function(x, y) {return x + y;}
    x => {return x + 1}
```

### Array destructuring
```javascript
    var [x, , y] = [1,2,3];             // x === 1, y === 3
    var [x] = [];                       // x === undefined
    var [x = 1] = [];                   // x === 1 (default value)
    var [x, y, z] = "xyz";              // x === "x", y === "y", z === undefined
    var [a, ...b] = [1, 2, 3];          // a === 1, b === [2, 3]
    var [a, ...b] = [1];                // a === 1, b === []
```

### Object destructuring
```javascript
    var {x, a:y, z} = {x: 1, y: 2};     // x === 1, a === 2, z === undefined
```

### Default function parameters
```javascript
    function(a = 1, b = 2) {...}
    function(a, b = a) {...}            // default can be previous param
```

### Rest parameters
```javascript
    function(a, ...b) {...}             // b will be an array containing the 2nd and above params
```

### Template strings
```javascript
    var x = 1, y = 'hello';
    `${y}! x + 1 = ${x + 1}`                      // === "hello! x + 1 = 2"
```

### Modules
```javascript
    export function duplicate(x) {return x + x;}
    export var name = 'mi';
    
    import * as mylib from "lib/mylib"
    mylib.duplicate(mylib.name);        // === 'mimi'
    
    import { duplicate, name } from "lib/math";
    duplicate(name);                    // === 'mimi'
```

### Classes
```javascript
    class Rect {
        constructor (x, y) {
        	this.x = x;
        	this.y = y;
        }
        area() {return this.x + this.y;}
    }
```

### Promises
```javascript
	var promise = new Promise(
    	function (resolve, reject) {
    		success ? resolve(value) : reject(reason);
    	}
    });
    
    promise.then(
        function (value) { /* fulfillment */ },
        function (reason) { /* reject */}
    );
```

### Octal and binary literals
```javascript
    0b10101101                          // === 173
    0o255                               // === 173
```

### `Number` properties
```javascript
    Number.isFinite
    Number.isInteger
    Number.isSafeInteger
    Number.isNaN
    Number.EPSILON                      // 2.220446049250313e-16
    Number.MIN_SAFE_INTEGER             // -9007199254740991
    Number.MAX_SAFE_INTEGER             // 9007199254740991
```

### `Math` methods
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
