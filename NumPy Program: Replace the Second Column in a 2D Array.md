# NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program

```python
import numpy as np

rows = int(input("Enter the number of rows: "))
cols = int(input("Enter the number of columns: "))

print("Enter the elements of the 2D array row by row:")
array = []
for _ in range(rows):
    row = list(map(int, input().split()))
    array.append(row)

array = np.array(array)

print("Enter the new column (", rows, "values):")
new_column = []
for _ in range(rows):
    val = int(input())
    new_column.append(val)

new_column = np.array(new_column)

array = np.delete(array, 1, axis=1)
updated_array = np.insert(array, 1, new_column, axis=1)

print("\nUpdated array:")
print(updated_array)

```

## Output

![image](https://github.com/user-attachments/assets/552ec7ae-4457-41b6-bcfb-7c2c7df8178c)

## Result
Hence the program is executed successfully.
