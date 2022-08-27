# Python & Javascript Semantic Parallels

## Lambda & Anonymous Arrow Functions

## Higher Order Functions (map,reduce,filter)

### map

```py

def square(n):
    return n*n

nums = [1, 2, 3, 4, 5]
result = map(square,nums)

print(list(result)) #[1,4,9,16,25]

```

```js
function square(n) {
  return n * n;
}

let nums = [1, 2, 3, 4, 5];
let result = nums.map(square);

print(result); // [1,4,9,16,25]
```

### filter

```py
def isGreaterThan2(num):
    return num > 2

nums = [1,2,3,4,5]
result = filter(isGreaterThan2,nums)

print(list(result)) # [3,4,5]
```

```js
const nums = [1, 2, 3, 4, 5];

function isGreaterThan2(num) {
  return num > 2;
}

let result = nums.filter(isGreaterThan2);

console.log(result); // [3, 4, 5]
```

### reduce

```py
from functools import reduce

nums = [1, 2, 3, 4, 5]

def sum_(total, num):
    return total + num

result = reduce(sum_,nums)
print(result) # 15
```

```js
const nums = [1, 2, 3, 4, 5];

function sum(total, num) {
  return total + num;
}

let result = nums.reduce(sum, 0);

console.log(result); // 15
```

## List Comprehension & Spread Operator

## Unpacking & Object Destructuring

## .items() && object.entries()

## Swapping Variables

```py
first = "i am first";
second = "i am second";

# swapping the variables
first, second = second, first

print(first) # i am second
print(second) # i am first

```

```js
let first = "i am first";
let second = "i am second";

// swapping the variables
let [second, first] = [first, second];

console.log(first); // i am second
console.log(second); // i am first
```

## Module Imports

## Backticks && Docstrings

## Ternary

```py
age = 21

status = "you are qualified" if age > 18 else "you are not qualified"

print(status) # you are qualified
```

```js
const age = 21;

const status = age > 18 ? "you are qualified" : "you are not qualified";

console.log(status); // you are qualified
```
