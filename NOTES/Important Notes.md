___
- Python is a Dynamically Typed Language that means it infers data type from the Value. So one can reassign a variable to hold a value of completely different data type.
	For Eg-
```python
number = 1
number ="one"
``` 


- One can check the Datatype of a Function using `type` function
  ```python
  number = 19
  print(type(number))
  ```


- Lists are ordered collections of items—enclosed within a pair of square brackets. The items in a list can all be of the same or different data types. Lists are _mutable_, meaning you can change their content after creation.
  
  Here, `student_names` contains the names of students:
  ```python
  # List
  student_names = ["Alice", "Bob", "Charlie", "David"]
  ```
  
  
- Tuples are ordered collection similar to list(besides using `()` brackets instead of `[]` ) and are basically immutable after creation. Thus Data inside cannot be changed further.

   Say you want `student_scores` to be an immutable collection that contains the exam scores of students.
   ```python
   # Tuple
   student_scores = (85, 90, 45, 88)
   ```


- Dictionaries are collections of key-value pairs. The keys of a dictionary should be unique, and they map to corresponding values. They are mutable and allow you to associate information with specific keys.
  
  Here, `student_info` contains information about each student—names and scores—as key-value pairs:
  
  ```python
  # Dictinary
  student_info = {'Alice': 85, 'Bob': 92, 'Charlie': 78, 'David': 88}
  ```

- Another built-in Python data type is the `set`, which stores an _un-ordered_ list of _unique_ items. Being unordered, sets do not record element position or order of insertion and so do not support indexing.
  
  ```python
  s = { 2, 5, 7, 11}
  s
  ```
  
  ```
  # Output
  {2, 5, 7, 11}
  ```

---

```python
{1, 2, 3} == {3, 2, 1}
```

```
 # Output
 True
```

---

```python
[1, 2, 3] == [3, 2, 1]
```

```
  # Output
  False
```

---

```python
s.add(2)  # does nothing
s
```

```
# Output
{2, 5, 7, 11}
```

---

```python
s[0]
```

```
---------------------------------------------------------------------------
TypeError                                 Traceback (most recent call last)
<ipython-input-93-c9c96910e542> in <module>
----> 1 s[0]

TypeError: 'set' object is not subscriptable
```


---

## Question Practice

1. Takes an integer n and prints the sum of numbers from 1 to n using a for loop.
   
   ```python
   def sum_of_numbers(n):
    total = 0
    for i in range(1, n + 1):
        total += i
    return total

print("Sum of numbers from 1 to 10 is:", sum_of_numbers(10))
   ```
   
   
2. Using a while loop, keep taking input until the user enters "stop", then print how many valid inputs (not "stop") were given.
   
   ```python
   def count_inputs():
    count = 0
    while True:
        user_Input = input("Enter something (type 'stop' to end): ")
        if user_Input.lower() == "stop":
            break
        else:
            count += 1
    print("Number of valid inputs till 'stop':", count)

count_inputs()
   ```
