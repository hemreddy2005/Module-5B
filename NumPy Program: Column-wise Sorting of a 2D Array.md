# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program

```python
import numpy as np

rows = int(input("Enter the number of rows: "))
cols = int(input("Enter the number of columns: "))
array = []

print("Enter the elements row by row:")

for _ in range(rows):
    row = list(map(int, input().split()))
    array.append(row)

array = np.array(array)
sorted_array = np.sort(array, axis=0)

print("\nOriginal array:")
print(array)

print("\nColumn-wise sorted array:")
print(sorted_array)
```

## Output

![image](https://github.com/user-attachments/assets/7be99d11-86d4-4f15-b3d7-79fccc2d6c09)

## Result
Hence the program is executed successfully.
