# Classes and Objects in Python: Calculate the Area of a Circle

## 🎯 Aim
To write a Python program that calculates the **area of a circle** based on the radius provided by the user. This program uses a class named `pen` and a method `stationary` to perform the calculation.

## 🧠 Algorithm
1. **Get user input**: Take the radius of the circle as input from the user.
2. **Define the class**: Create a class named `pen`.
3. **Define the method**: Inside the class, define the method `stationary` to calculate the area of the circle using the formula:  
   Area = pi *r^2 
4. **Execute the program**: Create an object of the class and call the method with the radius value.

## 🧾 Program
``` python
import math
class pen:
    def stationary(self,r):
        return math.pi*r*r
r=int(input())
h=pen()
print("Area of circle:",round(h.stationary(r),2))
```

## Output
![image](https://github.com/user-attachments/assets/84e29a69-13e8-401b-8d27-358159c8b247)

## Result
Thus Python program that calculates the **area of a circle** is executed successfully.

## Dictionary Operations in Python: Merging Two Dictionaries

## 🎯 Aim
To Write a Python program to convert them into a dictionary in a way that item from list1 is the key and item from list2 is the value. Get two lists as input.

## 🧠 Algorithm
1.Start

2.Prompt the user to input a list of keys (e.g., ['a', 'b', 'c'])

3.Store the input in a variable called keys

4.Prompt the user to input a list of values (e.g., [1, 2, 3])

5.Store the input in a variable called values

6.Convert the keys input string to an actual list using eval() or ast.literal_eval()

7.Convert the values input string to an actual list

8.Combine the keys and values into pairs using the zip() function

9.Create a dictionary from the zipped pairs using the dict() function

10.Print the resulting dictionary

11.End
## 🧾 Program
``` python
keys = input()
values = input()
keys_list = eval(keys)
values_list = eval(values)
result = dict(zip(keys_list, values_list))
print(result)
```

## Output
![image](https://github.com/user-attachments/assets/200b8898-ca1e-4101-a571-650bd5daf6fd)

## Result
Thus the python program to convert the input into dictionary is executed successfully.

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
``` python
def sort_dict_by_values(d):
    return sorted(d.items(), key=lambda item: item[1])
my_dict = {3: 323,2: 56,4: 24, 6: 18,5: 12, 1: 2}
sorted_items = sort_dict_by_values(my_dict)
print("Keys and Values sorted in alphabetical order by the value")
print(sorted_items)

```

## Sample Output
![image](https://github.com/user-attachments/assets/e432bc44-1ec9-439d-8c4a-0801d6b29c30)

## Result
Thus the  Python program to sort a dictionary is executed successfully.

# Exception Handling in Python: Avoiding Index Errors

## 🎯 Aim
To write a Python program that handles an **IndexError** when trying to access an element beyond the available range of a list.

## 🧠 Algorithm
1.Start

2.Initialize an empty list a

3.Read an integer n from the user (number of elements to input)

4.Repeat the following n times:

a. Read an integer from the user

b. Append the integer to list a

5.Print the entire list a

6.Try to access and print the element at index 10 (11th element) from list a

7.If accessing index 10 causes an IndexError:

a. Print a message saying that the 11th element is not available (e.g., "10 is not accepted")

8.End


## 🧾 Program
``` python
try:
    a = []
    n = int(input())
    for i in range(n):
        b=int(input())
        a.append(b)
    print(a)
    print(a[10])
  

except IndexError:
   
    print("10 is not accepted")
```
## Output
![image](https://github.com/user-attachments/assets/bdc74ae9-6d48-431f-adda-801a0cfd739a)

## Result
Thus the a Python program that handles an **IndexError** is executed successfully.

# File Handling in Python: Count Lines Not Starting with 'T'

## 🎯 Aim
To write Python function to find and replace a word in a file.

## 🧠 Algorithm
1.create_file(file_path, content)
Purpose: Creates a file and writes the specified content into it.

Opens the file in write mode ('w')—this overwrites the file if it already exists.

Writes the content into the file.

2. find_and_replace(file_path, old_word, new_word)
Purpose: Finds all instances of old_word in the file and replaces them with new_word.

How it works:

Opens the file in read mode, reads all contents.

Replaces all occurrences of old_word with new_word.

Opens the file in write mode and writes the updated content back.

3. read_file(file_path)
Purpose: Reads and returns the contents of a file.

How it works:

Opens the file in read mode and returns the entire content as a string

## 🧾 Program
``` python
def create_file(file_path, content):
    with open(file_path, 'w') as file:
        file.write(content)
def find_and_replace(file_path, old_word, new_word):
    with open(file_path,'r')as f:
        cr=f.read()
        l=cr.replace(old_word,new_word)
    with open(file_path,'w') as f:
        f.write(l)


def read_file(file_path):
    with open(file_path, 'r') as file:
        return file.read()
```
## Output
![image](https://github.com/user-attachments/assets/3cce9630-0e78-46ae-8047-d13e862e936c)

## Result
Thus the  Python function to find and replace a word in a file is executed successfully.
