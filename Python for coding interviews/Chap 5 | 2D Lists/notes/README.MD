# 2D Lists

## Looping through a 2D List

```python
nested_list = [[1],[2,3],[4,5,6]]
for sublist in nested_list:
  for element in sublist:
    print(element)
```

## 2D Grid 

```python
grid =[
  [0,0,0],
  [0,0,0]
]

rows = len(grid)    #2
cols = len(grid[0]) #3
```

## Nested List Comprehension 

```python
grid = [[0 for i in range(3)] for j in range(2)]

```

```python
`print(grid)` ➡️  [
  									[0,0,0],
  									[0,0,0]
                   ]
```

Better Concise solution ➡️

```python
grid = [[0] * 3 for _ in range(2)]
```

- We create a list of zeroes with `[0] * 3` and use it for the outer list with list comprehension.Since the variable in the for loop is not used , we use an underscore `_` to indicate that it is a throwaway variable .This is a common convention in Python