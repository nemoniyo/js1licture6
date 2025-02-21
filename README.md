"# js1licture6" 

# Array, Destructuring, Spread, and Rest in JavaScript

This guide provides a concise overview of arrays, destructuring, and the spread/rest operators in JavaScript, with practical examples.

## Arrays

Arrays in JavaScript are used to store ordered collections of elements. They can contain elements of any type, including other arrays and objects.

```javascript
const numbers = [1, 2, 3, 4, 5];
const mixedArray = [1, 'two', { three: 3 }, [4]];
```

## Destructuring

Destructuring allows you to extract values from arrays or objects and assign them to variables.

### Array Destructuring

```javascript
const [a, b, c] = [3, 4, 5];
console.log(a, b, c); // Output: 3 4 5
```

Swap variables using destructuring:

```javascript
let x = 1;
let y = 2;
[x, y] = [y, x];
console.log(x, y); // Output: 2 1
```

### Object Destructuring

```javascript
const person = { name: 'Alice', age: 25 };
const { name, age } = person;
console.log(name, age); // Output: Alice 25
```

## Spread Operator

The `...` (spread) operator allows you to expand elements of an array or properties of an object.

### With Arrays

```javascript
const arr1 = [1, 2, 3];
const arr2 = [...arr1, 4, 5];
console.log(arr2); // Output: [1, 2, 3, 4, 5]
```

### With Objects

```javascript
const obj1 = { a: 1, b: 2 };
const obj2 = { ...obj1, c: 3 };
console.log(obj2); // Output: { a: 1, b: 2, c: 3 }
```

## Rest Operator

The `...` (rest) operator is used to collect remaining elements into an array or object.

### In Functions

```javascript
function sum(...numbers) {
  return numbers.reduce((acc, num) => acc + num, 0);
}

console.log(sum(1, 2, 3)); // Output: 6
```

### In Destructuring

```javascript
const [first, ...rest] = [1, 2, 3, 4];
console.log(first); // Output: 1
console.log(rest);  // Output: [2, 3, 4]
```

## Conclusion

Understanding arrays, destructuring, and the spread/rest operators is essential for efficient data manipulation in JavaScript. These tools enable you to write cleaner and more readable code.

