# Python Magic

## Ranges

```py
if x > 0 and x < 100:
    pass
```

```py
# refatored
if 0 < x < 100:
    pass
```

---

## Assignments

```py
# swapping values

x,y = y, x
```

```py
# unpacking

x,y = [1,2]
```

```py
x = 0
y = 0
k = 0

x = y = k = 0

```

---

## Ternary

```py
if y < 21: result = x
else: result = y
```

```py
result = x if y < 21 else y
```

---

## List Comprehension

```py

nums = [1,2,3,4,5,6]

even_nums = []

for num in nums:
    if num%2 == 0:
        even_nums.append(num)
```

```py

nums = [1,2,3,4,5,6]

even_nums = [num for num in nums if num%2 == 0]

```

```py
# SQUARE EVEN NUMBERS, CUBE ODD NUMBERS

# brute
nums = [1,2,3,4,5]
result = []

for num in nums:
    if num%2 == 0:
        result.append(num ** 2)
    else:
        result.append(num ** 3)

# refactored
nums = [1,2,3,4,5,6]

result = [num**2 if num%2 ==0 else num**3 for num in nums]

```

```py
# REMOVE DUPLICATES

x = [1,2,5,1,7,3,2,5,9,3]

no_duplicates = {num for num in nums}

```
