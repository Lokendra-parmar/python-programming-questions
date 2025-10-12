---
title: Problem-Solving: Factorial
---

# Problem Statement

Write a function to calculate the factorial of a non-negative integer. The factorial of a number is the product of all positive integers up to that number.

You need to implement the following function:

- `factorial(n: int) -> int`: Calculates the factorial of a non-negative integer `n`.

**Example**
```
print(factorial(5))  # Output: 120
```

# Solution

```py3 test.py -r 'python test.py'
<template>
def factorial(n: int) -> int:
    '''
    Calculate the factorial of a non-negative integer.

    Arguments:
    n: int - A non-negative integer.

    Return: int - The factorial of n.
    '''
    <los>...</los>
    <sol>
    if n == 0:
        return 1
    else:
        return n * factorial(n - 1)
    </sol>
</template>
<suffix_invisible>
{% include '../function_type_and_modify_check_suffix.py.jinja' %}
</suffix_invisible>
```

# Public Test Cases

## Input 1

```
is_equal(factorial(5), 120)
is_equal(factorial(0), 1)
```

## Output 1

```
120
1
```

# Private Test Cases

## Input 1

```
is_equal(factorial(7), 5040)
is_equal(factorial(1), 1)
```

## Output 1

```
5040
1
```