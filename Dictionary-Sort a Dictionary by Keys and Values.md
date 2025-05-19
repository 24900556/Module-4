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
