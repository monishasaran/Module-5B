# 1.NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program
```
import numpy as np
arr=np.array(eval(input()))
print("Given array")
print(arr)
print()
print(np.sort(arr,axis=0))
```
## Output
<img width="563" height="405" alt="image" src="https://github.com/user-attachments/assets/ee84b186-ce58-4d7b-b7b0-6ac9e42f178a" />


## Result
Thus, the program to sort a 2D NumPy array column-wise was executed successfully.

# 2.NumPy Program: Find Indices Where Elements in Array x are Greater Than or Equal to Corresponding Elements in Array y

🎯 Aim

To write a Python program using NumPy that finds the indices where elements in array x are greater than or equal to their corresponding elements in array y.

🧠 Algorithm

Import NumPy: Import the NumPy library.
Define Arrays: Define two NumPy arrays, x and y, with the same shape (i.e., same number of elements).
Use Boolean Indexing:
x > y gives a boolean array where elements of x are greater than y.
x == y gives a boolean array where elements of x are equal to y.
Find Indices: Use np.where() to get the indices where the conditions x >= y are satisfied.
Print Indices: Print the indices where the condition holds true.

🧾 Program
```
import numpy as np
a=np.array(eval(input()))
b=np.array(eval(input()))
x=np.where(a>b)
print(x)
y=np.where(a==b)
print(y)
```
Output:

<img width="942" height="192" alt="image" src="https://github.com/user-attachments/assets/e5bd83e0-b659-4594-8f0f-a183e30b4704" />


Result:

Thus, the program to find indices where elements in array x are greater than or equal to corresponding elements in array y was executed successfully.

# 3.NumPy Program: Replace the Second Column in a 2D Array

## 🎯 Aim
To write a **NumPy** program that deletes the second column from a given 2D array and inserts a new column at the same position.

## 🧠 Algorithm
1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Get a 2D NumPy array and a new column (as another array) from the user.
3. **Delete Column**: Use `np.delete()` to remove the second column (index 1) from the original array.
4. **Insert Column**: Use `np.insert()` to insert the new column at the second column's original position.
5. **Display Result**: Print the updated array with the replaced column.

## 🧾 Program
```
import numpy as np
x=np.array(eval(input()))
y=np.array(eval(input()))
print("Printing Original array")
print(x)
result=np.delete(x, 1,axis=1)
print("Array after deleting column 2 on axis 1")
print(result)
result=np.insert(result,1,y,axis=1)
print("Array after inserting column 2 on axis 1")
print(result)
```
## Output

<img width="1131" height="681" alt="{994E3092-442F-4D26-AD6B-D94592026757}" src="https://github.com/user-attachments/assets/21b35ffb-e8f1-4c1e-be6f-4b049be1e034" />


## Result
Thus, the program to create and display a Pandas DataFrame with custom index labels was executed successfully.

# 4.Pandas Program: Create and Display a DataFrame with Custom Index Labels

## 🎯 Aim

To create and display a **DataFrame** using the **Pandas** library in Python from a given dictionary, and apply specific index labels to the rows.


## 🧠 Algorithm

1. **Import Libraries**: Import the required libraries – `pandas` and `numpy`.
2. **Create Dictionary**: Define a dictionary `exam_data` with keys: `'name'`, `'score'`, `'attempts'`, and `'qualify'`.
3. **Index Labels**: Create a list of custom index labels called `labels`.
4. **Create DataFrame**: Use `pd.DataFrame()` to create the DataFrame by passing the dictionary and index labels.
5. **Display Output**: Display the DataFrame using `print()` or by simply calling the DataFrame variable.



## 💻 Program
```
import numpy as np
import pandas as pd
exam_data=eval(input())
lab=np.array(eval(input()))
df=pd.DataFrame(exam_data,index=lab)
print(df)
```
## Output
<img width="948" height="246" alt="image" src="https://github.com/user-attachments/assets/c10a3f8d-0ed2-42ec-b8be-c6bf5237b33f" />

## Result
Thus, the program to create and display a Pandas DataFrame with custom index labels was executed successfully.

#  5. Pandas Program: Join Two DataFrames Along Rows

## 🎯 AIM

To write a Python program using Pandas to **join two DataFrames along rows** (row-wise concatenation) and assign all data to a new DataFrame.


## 🧠 ALGORITHM

1. **Import Libraries**: Import the `pandas` library.
2. **Create First DataFrame**: Use a dictionary to create `student_data1`.
3. **Create Second DataFrame**: Use another dictionary to create `student_data2`.
4. **Concatenate DataFrames**: Use `pd.concat()` with `axis=0` to concatenate both DataFrames row-wise.
5. **Display Result**: Print the new combined DataFrame.


## 💻 Program

```
import pandas as pd
dict1 = eval(input())
dict2 = eval(input())
df1 = pd.DataFrame(dict1)
df2 = pd.DataFrame(dict2)
print("Original DataFrames:")
print(df1)
print("-------------------------------------")
print(df2)
joined_df = pd.concat([df1, df2], axis=0)

print("\nJoin the said two dataframes along rows:")
print(joined_df)
```

## Output
<img width="1119" height="676" alt="Screenshot 2025-10-20 154259" src="https://github.com/user-attachments/assets/c6a75b2d-26b5-4301-b9e1-b3cc6f33c907" /><img width="813" height="773" alt="Screenshot 2025-10-20 154622" src="https://github.com/user-attachments/assets/d1988b1a-4a7b-4fa1-9699-75457201d28d" />


## Result
Thus , the program has been executed succesfully.
