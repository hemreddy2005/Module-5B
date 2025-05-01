# 🧪 Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.

---

## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.

---

## 💻 Program

```python
import pandas as pd

student_data1 = {
    'name': ['Alice', 'Bob'],
    'score': [85, 90],
    'attempts': [1, 2],
    'qualify': ['yes', 'no']
}

student_data2 = {
    'name': ['Charlie', 'David'],
    'score': [78, 88],
    'attempts': [2, 1],
    'qualify': ['yes', 'yes']
}

df1 = pd.DataFrame(student_data1)
df2 = pd.DataFrame(student_data2)

new_df = pd.concat([df1, df2], axis=0)

print(new_df)
```

## Output

![image](https://github.com/user-attachments/assets/069ac45b-87aa-4c52-8dc7-d51792450e64)

## Result
Hence the program is executed successfully.
