# Functions 

## Introduction to Functions

```python
def greet():
    print("Hello , world!")
```

## Parameters

```python
def greet(name):
    msg = "Hello ", + name
    print(msg)
    
greet("Alice") # This will print "Hello, Alice"
```

## Multiple Parameters 

```python
def greet(name,greeting):
    message = greeting + " " + name
    print(msg)
    
greet("Alice","Hello") # This will print "Hello ,Alice"
```

## Return Statement 

```python
def add(x,y):
    return x + y
result = add(3,5)
print(result) #This will print 8
```

## Type Hints 

```python
def add(x:int,y:int) -> int:
    return x + y
```

## Default Arguments 

```python
def greet(name="world"):
    print("Hello"+name+"!")
greet() # This will print "Hello , world!"
greet("Bob") # This will print "Hello , Bob!"
```

