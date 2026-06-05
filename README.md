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
import numpy as np
arr=np.array(eval(input()))
print("Given array")
print(arr)
print()
print(np.sort(arr,axis=0))

## Output
<img width="857" height="561" alt="image" src="https://github.com/user-attachments/assets/1ee05616-298c-471a-a2e7-fa8f760ab58e" />


## Result
Thus, the program to sort a 2D NumPy array column-wise was executed successfully.


# # NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

## 🎯 Aim
To write a Python program using **NumPy** that finds the indices where elements in array `x` are greater than or equal to their corresponding elements in array `y`.

## 🧠 Algorithm
1. **Import NumPy**: Import the NumPy library.
2. **Define Arrays**: Define two NumPy arrays, `x` and `y`, with the same shape (i.e., same number of elements).
3. **Use Boolean Indexing**: 
   - `x > y` gives a boolean array where elements of `x` are greater than `y`.
   - `x == y` gives a boolean array where elements of `x` are equal to `y`.
4. **Find Indices**: Use `np.where()` to get the indices where the conditions `x >= y` are satisfied.
5. **Print Indices**: Print the indices where the condition holds true.

## 🧾 Program
import numpy as np
a=np.array(eval(input()))
b=np.array(eval(input()))
x=np.where(a>b)
print(x)
y=np.where(a==b)
print(y)

## Output
<img width="1025" height="197" alt="image" src="https://github.com/user-attachments/assets/dcf1c1ee-c857-446a-8e6e-1473394e8fd3" />


## Result
Thus, the program to find indices where elements in array x are greater than or equal to corresponding elements in array y was executed successfully.


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
import numpy as np
import pandas as pd
exam_data=eval(input())
lab=np.array(eval(input()))
df=pd.DataFrame(exam_data,index=lab)
print(df)

## Output
<img width="1037" height="247" alt="image" src="https://github.com/user-attachments/assets/72008cf8-31f1-485e-be1f-1859ce632975" />


## Result
Thus, the program to create and display a Pandas DataFrame with custom index labels was executed successfully.


# Pandas Program: Create and Display a DataFrame with Custom Index Labels

## 🎯 Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.

---

## 🧠 Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.

---

## 💻 Program
import numpy as np
import pandas as pd
exam_data=eval(input())
lab=np.array(eval(input()))
df=pd.DataFrame(exam_data,index=lab)
print(df)

## Output
<img width="1042" height="257" alt="image" src="https://github.com/user-attachments/assets/709c8eb9-b484-4141-82d2-b49f84bef9a5" />

## Result
Thus, the program to create and display a Pandas DataFrame with custom index labels was executed successfully.


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
import pandas as pd
a=eval(input())
b=eval(input())
df1=pd.DataFrame(a)
df2=pd.DataFrame(b)
print("Original DataFrames:")
print(df1)
print("-------------------------------------")
print(df2)
print()
mer=pd.concat([df1,df2])
print("Join the said two dataframes along rows:")
print(mer)

## Output
<img width="1037" height="622" alt="image" src="https://github.com/user-attachments/assets/f6fd5d75-4631-4e45-9f64-46c20c815666" />


## Result
Thus, the program to join two Pandas DataFrames along rows was executed successfully.
