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
