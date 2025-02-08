# Lambda Functions in Python
### What is a Lambda Function?
- A lambda function in Python is an anonymous function that is defined using the lambda keyword.
- It can take multiple arguments but has only one expression.


Syntax
```python
  lambda arguments: expression
```

1. Basic Example
```python
add = lambda x, y: x + y
print(add(5, 3))  # Output: 8
```

2. Creating a Multiplication Table
```python
multiplication_table = lambda n: [n * i for i in range(1, 11)]

print(multiplication_table(5))  
# Output: [5, 10, 15, 20, 25, 30, 35, 40, 45, 50]

```

3. Flattening a Nested List
```python
flatten = lambda lst: [item for sublist in lst for item in sublist]

print(flatten([[1, 2], [3, 4], [5, 6]]))  # Output: [1, 2, 3, 4, 5, 6]

```

## Rules for Lambda Functions in Python

1️⃣ Must Have Only One Expression
- A lambda function cannot have multiple expressions or statements.
- It evaluates a single expression and returns the result automatically.
  
2️⃣ No Assignments Inside Lambda
- You cannot use the = operator inside a lambda function.
- If you need a variable assignment, use a normal function instead.
  
3️⃣ Can Take Any Number of Arguments
- A lambda function can accept multiple arguments, but it can only evaluate one expression.
  
4️⃣ Cannot Have return, while, for, or try-except
- You cannot use return (implicit return is always used).
- Loops like for and while are not allowed inside a lambda.
- Exception handling (try-except) is not possible.



