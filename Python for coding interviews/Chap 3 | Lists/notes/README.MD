# Lists 

## Useful List Operations 

### `append()`

- adds an element to the end of the list 

- Time Complexity :O(1)

  ```python
  my_list =[1,2,3]
  my_list.append(4)
  print(my_list) # [1,2,3,4]
  ```

### `pop()`

- removes and returns the last element of the list 

- if the list is already empty we will get an Error (IndexError)

- We can pass an integer to pop() to remove an element at a specified index 

- If we pop(index) an index that is out of bounds we will get an error (IndexError)

- Time Complexity : O(1)

  ```python
  my_list =[1,2,3,4]
  my_list.pop()
  print(my_list) # [1,2,3]
  my_list.pop(0)
  print(my_list) # [2,3]
  ```

### `insert()`

- inserts an element at a specified index in the list

- syntax ➡️ `insert(index, element)` 

- If the index is too large the element will be inserted at the end of the list 

- Time Complexity : O(n)

  ```python
  my_list =[1,2,3,4]
  my_list.insert(1,5)
  print(my_list) # [1,5,2,3,4]
  my_list.insert(10,35)
  print(my_list) # [ 1,5,2,3,4,35]
  
  ```

### `index()`

- returns the index of the first occurance of a specified element in the list 

- if the element is not in the list we will get an error (ValueError)

- Time Complexity :O(n)

  ```python
  my_list =[1,2,3,4]
  print(my_list.index(2)) # 1
  ```

### `remove()`

- removes the first occurance of a specified element from the list 

- Time Complexity :O(n)

  ```python
  my_list =[1,2,3,4]
  my_list.remove(2) 
  print(my_list) # [1,3,4]
  ```

### `extend()`

- Adds the elements of another list to the end of the list 

- It modifies the original list 

- Time Complexity :O(m) where m is the length of the list passed to `extend()`

  ```python
  my_list1 =[1,2,3,4]
  my_list2 = [5,6]
  my_list1.extend(my_list2) 
  print(my_list1) # [1,2,3,4,5,6]
  print(my_list2) # [5,6]
  ```

### `in` operator 

- If we want to check if an element is in a list we can use the `in` operator 

- Time Complexity ➡️  O(n) where n is the length of the list 

  ```python
  my_list = [1,2,3]
  if 3 in my_list:
    print("3 is in the list")
  ```

### list concat with `+` operator 

- The `+` operator creates a new list 

- Time Complexity ➡️ O(n+m) where n is the length of one list and m is the length of the other list 

  ```python
  my_list1 =[1,2,3,4]
  my_list2 = [5,6]
  result = my_list1 + my_list2 
  print(my_list1) # [1,2,3,4]
  print(my_list2) # [5,6]
  print(result) # [1,2,3,4,5,6]
  ```

### List initialization 

```python
my_list1 = [0] * 5 # The above code will create a list of 5 zeroes
my_list2 = [1] * 3 # The above code will create a list of 3 ones
```

## List clone

- There are 3 ways by which we can do shallow copy(`.copy()` , `slice` , `list()` constructor ) of lists . If we have a list of integers which are primitive types we dont need to worry about shallow copy or deep copy .  But if we have a list of objects we have to use deep copy with `copy.deepcopy(my_list)`

- Shallow copy with `copy()` , `slicing` and `list()` constructor 

  ```python
  original_list1 = [1,2,3]
  cloned_list1 = original_list1.copy()
  print(cloned_list1) #[1,2,3]
  
  original_list2 =[1,2,3,4]
  cloned_list2 = original_list2[:]
  print(original_list2) # [1,2,3,4]
  
  original_list3 = [1,2,3,4,5]
  cloned_list3 = list(original_list3)
  print(cloned_list3) # [1,2,3,4,5]
  ```

- Deep copy with `copy.deepcopy(my_list)`

  ```python
  import copy 
  original_list = [[1,2],[3,4]]
  cloned_list = copy.deepcopy(original_list)
  ```

## List Comprehension 

- allows us to create lists in a concise way 

- Example 1 ➡️

  ```python
  my_list = [i for i in range(5)]
  print(my_list) #[0,1,2,3,4]
  
  ```

  - in the above example we have a for loop inside the square brackets .The loop iterates over the range of numbers from 0-4 .Before the loop we place the expression i which is th value we want to add to the list 

- Example 2 ➡️

  ```python
  arr1 = [1,2,3]
  arr2 = [4,5,6]
  result = [i+j for i,j in zip(arr1,arr2)]
  print(result) # [5,7,9]
  ```

  - We have 2 lists arr1 and arr2 .We use the `zip()` function to iterate over both lists at the same time .We then add the elements of both lists together and create a new list .The expression `i+j` is the value we want to add to the list

- Example 3 ➡️

  ```python
  arr= [1,2,3,4,5]
  
  result = [i for i in arr if i%2 ==0] #[2,4]
  ```

