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
