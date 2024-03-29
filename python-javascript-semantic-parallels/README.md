# Python & Javascript Semantic Parallels

> ## 1. Lambda & Anonymous Arrow Functions

```py
sum_pair = lambda x,y : x + y

print(sum_pair(5,3)) # 8
```

```js
let sum_pair = (x, y) => x + y;

console.log(sum_pair(5, 3)); // 8
```

> ## 2. Higher Order Functions (map,reduce,filter)

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

> ## 3. List Comprehension & Spread Operator

```js
const A = [1, 2, 3, 4, 5];
const B = [...A];

console.log(B); // [1,2,3,4,5]
```

```py
A = [1,2,3,4,5]
B = [num for num in A]

print(B) # [1,2,3,4,5]
```

> ## 4. \*Args & Rest Operator

```py
def multiply(*nums):
  product = 1

  for num in nums:
    product *= num

  return product
```

```js
function multiply(...nums) {
  let product = 1;

  for (num of nums) {
    product *= num;
  }

  return product;
}
```

> ## 5. Unpacking & Object Destructuring

```py
student = ["Dolores Abernathy", 21]
name,age = student

print(name) # Dolores Abernathy
print(age)  # 21
```

```js
const student = ["Dolores Abernathy", 21];

const [name, age] = student;

console.log(name); // Dolores Abernathy
console.log(age); // 21
```

> ## 6. items() && object.entries()

```js
const student = {
  name: "Dolores Abernathy",
  age: 21,
};

const result = Object.entries(student);
console.log(result);
// [ ["name","Dolores Abernathy"], ["age",21] ]

for (let [key, value] of Object.entries(student)) {
  console.log(key + " -> " + value);
}
```

```py
student = {
    'name': 'Dolores Abernathy',
    'age': 21
}

print(list(student.items()))
# [('name', 'Dolores Abernathy'), ('age', 21)]

for key,value in student.items():
    print(key + " -> " + value)

```

> ## 7. Swapping Variables

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

> ## 8. Module Imports

### namespace imports

```py
import greetings

print(greetings.hello)
```

```js
import * as greetings from "./greetings.js";

console.log(greetings.hello);
```

### importing one item

```py

from greetings import hello

print(hello)

```

```js
import hello from "./greetings.js"; // for default exports
import { hello } from "./greetings.js"; // for named exports
```

### importing multiple items

```py
from greetings import hello, hi
```

```js
import { hello, hi } from "./greetings.js";
```

### importing with aliases

```py
from greetings import hello as hell, hi as hy
```

```js
import { hello as hell, hi as hy } from "./greetings.js";
```

> ## 9. Backticks && Docstrings

both render multiline strings

```py
name = "Faddal Ibrahim"

print("""hello {}""".format(name))
```

```js
let name = "Faddal Ibrahim";

console.log(`hello ${name}`);
```

> ## 10. Ternary

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
