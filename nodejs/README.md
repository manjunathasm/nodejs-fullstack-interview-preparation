# NodeJS Concepts, Quetions and Answers

### Data Types in Node.js

Node.js is built on top of JavaScript, so it shares the same fundamental data types as JavaScript. However, since Node.js is server-side, it also includes additional types specific to its environment (like Buffer).

- Primitive Data Types:

  - String: Represents textual data.

    ```javascript
    const name = "John";
    ```

  - Number: Represents both integer and floating-point numbers.

    ```javascript
    const age = 30;
    const pi = 3.14;
    ```

  - Boolean: Represents a logical entity having two values: true or false.

    ```javascript
    const isActive = true;
    ```

  - Undefined: Represents a variable that has been declared but has not been assigned a value.

    ```javascript
    let address;
    console.log(address); // undefined
    ```

  - Null: Represents the intentional absence of any object value.

    ```javascript
    const data = null;
    ```

  - Symbol: Represents a unique and immutable primitive value and may be used as the key of an object property.

    ```javascript
    const uniqueID = Symbol("id");
    ```

- Non-Primitive Data Types:
  - Object: Represents a collection of key-value pairs.

    ```javascript
    const user = {
        name: "Alice",
        age: 28,
    };
    ```

  - Function: A block of code designed to perform a particular task.

    ```javascript
    function greet() {
        console.log("Hello");
    }
    ```

- Node.js-Specific Data Types:
  - Buffer: Represents raw binary data and is mainly used to handle binary data, such as reading from files or handling network packets.

    ```javascript
    const buf = Buffer.from("Hello");
    console.log(buf); // <Buffer 48 65 6c 6c 6f>
    ```

  - Stream: Used to handle streaming data like reading and writing files, network communications, etc.

    ```javascript
    const fs = require('fs');
    const readableStream = fs.createReadStream('file.txt');
    ```

  - BigInt: Represents whole numbers larger than 2^53 - 1, which is the largest number JavaScript can reliably represent with the Number primitive.

    ```javascript
    const bigNumber = 123456789012345678901234567890n;
    ```
