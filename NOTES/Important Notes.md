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
  