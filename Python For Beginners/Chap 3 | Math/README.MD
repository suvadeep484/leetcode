# Math 

## Arithmatic Operators 

| Arithmatic operator   | What it does ?                                               |
| --------------------- | ------------------------------------------------------------ |
| `+`                   | adds 2 operands together                                     |
| `-`                   | substracts the second operator from the first                |
| `*`                   | multiplies 2 operands                                        |
| `/`                   | divides the first operand by the second . the result is always a float |
| `//` (Floor division) | divides the first operand by the second and rounds down the result to an integer |
| `%` (Modulas)         | Returns the remainder of the division of the first operand by the second |
| `**` Exponentiation   | Raises the first operand to the power of the second operand  |

## Shorthand Operators 

```python
count = 0
count += 1
count += 2
print(count)  # Output: 3

```

- The `+=` operator is shorthand for `count = count + `. The other arithmetic operators have similar shorthand operators:
  - `-=` is shorthand for `count = count -`
  - `*=` is shorthand for `count = count *`
  - `/=` is shorthand for `count = count /`
  - `%=` is shorthand for `count = count %`
  - `//=` is shorthand for `count = count //`
  - `**=` is shorthand for `count = count **`

## Boolean operands 

- Boolean or ➡️ The or operator returns True if at least one of the operands is `True` .This holds even if we have more than two operands 

  ```pyt
  a,b,c = False , False , True 
  print(a or b or c) # Output : True
  ```

- Boolean and ➡️ The and operator returns True if all of the operands is True . This also holds if we have more than two operands 

  ```pyt
  a,b,c = True, True , True 
  print(a and b and c) #output : True
  ```

- Boolean not ➡️ inverts the value of the operand . If the operand is True , the result is False .If the operand is False the result is True

