# Classes and Objects in Python: Calculate the Area of a Circle

## 🎯 Aim
To write a Python program that calculates the **area of a circle** based on the radius provided by the user. This program uses a class named `cse` and a method `mech` to perform the calculation.

## 🧠 Algorithm
1. **Get user input**: Take the radius of the circle as input from the user.
2. **Define the class**: Create a class named `cse`.
3. **Define the method**: Inside the class, define the method `mech` to calculate the area of the circle using the formula:  
   Area = pi *r^2 
4. **Execute the program**: Create an object of the class and call the method with the radius value.

## 🧾 Program
      import math
      class cse:
          def mech(self, radius):
              # Calculate area of the circle
              area = math.pi * (radius ** 2)
              print(f"Area of the circle with radius {radius} is: {area:.2f}")
      r = float(input("Enter the radius of the circle: "))
      circle = cse()
      circle.mech(r)


## Output
![Screenshot 2025-05-19 205401](https://github.com/user-attachments/assets/314a85d0-3c19-4a4e-80e0-ebde59bf45e0)

## Result
Thus, the program is verified successfully.

## Dictionary Operations in Python: Merging Two Dictionaries

## 🎯 Aim
To write a Python program that merges **two dictionaries** and combines their key-value pairs.

## 🧠 Algorithm
1. Define two dictionaries `dict1` and `dict2` with some key-value pairs.
2. Define a function `merge()` that merges the two dictionaries using the `**` unpacking operator.
   - The merged result will combine keys from both dictionaries. If a key exists in both, the value from `dict2` will overwrite that from `dict1`.
3. Call the `merge()` function and print the merged dictionary.

## 🧾 Program
      dict1 = {'a': 1, 'b': 2, 'c': 3}
      dict2 = {'b': 20, 'd': 4}
      def merge(d1, d2):
          # Merge using unpacking operator (**)
          merged_dict = {**d1, **d2}
          return merged_dict
      merged = merge(dict1, dict2)
      print("Merged dictionary:", merged)


## Output
![Screenshot 2025-05-19 205548](https://github.com/user-attachments/assets/dec2a01a-3e66-4541-9a7b-46fdeb3be6a5)

## Result
Thus, the program is verified successfully.

# 🔤 Dictionary-Python Program to Sort a Dictionary by Keys and Values

This Python program demonstrates how to sort a dictionary:
- Alphabetically by keys
- Alphabetically by values

---

## 🎯 Aim

To write a Python program that sorts a dictionary's:
- Keys in alphabetical order
- Values in alphabetical order

---

## 🧠 Algorithm

1. **Start the program.**
2. **Define** a dictionary with key-value pairs.
3. **Sort by Keys**:
   - Use `sorted(dictionary.items())`
   - Convert the result to a dictionary using `dict()`
4. **Sort by Values**:
   - Use `sorted(dictionary.items(), key=lambda item: item[1])`
   - Convert the result to a dictionary using `dict()`
5. **Display** the original and sorted dictionaries.
6. **End the program.**

---

## 🧪Program
      my_dict = {'banana': 'yellow', 'apple': 'red', 'grape': 'purple', 'cherry': 'red'}
      sorted_by_keys = dict(sorted(my_dict.items()))
      sorted_by_values = dict(sorted(my_dict.items(), key=lambda item: item[1]))
      print("Original dictionary:")
      print(my_dict)
      
      print("\nDictionary sorted by keys:")
      print(sorted_by_keys)
      
      print("\nDictionary sorted by values:")
      print(sorted_by_values)

## Sample Output
![Screenshot 2025-05-19 205808](https://github.com/user-attachments/assets/87f53efc-9386-4a32-b79e-584c98b01f60)

## Result
Thus, the program is verified successfully.

# Exception Handling in Python: Avoiding Index Errors

## 🎯 Aim
To write a Python program that handles an **IndexError** when trying to access an element beyond the available range of a list.

## 🧠 Algorithm
1. Define a list `list1` with some integer elements.
2. Use a **try-except** block:
   - In the `try` block, attempt to access an index that is out of range (e.g., `list1[5]`).
   - In the `except` block, catch the error and print a custom message `"You're out of list range"`.
3. Print the result based on whether the index access succeeds or fails.

## 🧾 Program

      list1 = [10, 20, 30]
      
      try:
          # Attempt to access an index that's out of range
          print("Accessing index 5:", list1[5])
      except IndexError:
          # Handle the error
          print("You're out of list range")

## Output
![Screenshot 2025-05-19 205936](https://github.com/user-attachments/assets/3ca3899a-ab41-4a37-95eb-c7b1bf13a42e)

## Result
Thus, the program is verified successfully.

# File Handling in Python: Count Lines Not Starting with 'T'

## 🎯 Aim
To write a Python program that counts the number of lines in a text file `story.txt` that do **not** start with the alphabet `'T'`.

## 🧠 Algorithm
1. Open the file `story.txt` in **read mode**.
2. Initialize a counter `count` to zero.
3. Iterate through each line of the file:
   - Check if the first character of the line is **not** `'T'`.
   - If the line does not start with `'T'`, increment the `count` by 1.
4. After processing all lines, print the `count` value, which represents the number of lines that do not start with `'T'`.

## 🧾 Program
      with open('story.txt', 'w') as file:
          file.write("This is the first line.\n")
          file.write("Another line starts here.\n")
          file.write("That’s yet another line.\n")
          file.write("One more line not starting with T.\n")
      
      with open('story.txt', 'r') as file:
          count = 0  
          for line in file:
              if not line.lstrip().startswith('T'):
                  count += 1  
      
      print("Number of lines that do not start with 'T':", count)

## Output
![Screenshot 2025-05-19 210433](https://github.com/user-attachments/assets/fd6821ca-727f-4737-8828-3b64df7f1ab4)

## Result
Thus, the program is verified successfully.
