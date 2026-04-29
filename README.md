# PyTorch Basics Exercises
# Name: Chiiradeep R
# Reg No: 212224240028

# AIM:
Write a Python program using PyTorch that performs the following tasks:

# Software Required:
Python 3.x

PyTorch

Jupyter Notebook (for interactive development and execution)

# Algorithm:
## Step 1:
Perform standard imports

Import torch and NumPy.
## YOUR CODE HERE
```py
import torch
import numpy as np
```
## Step 2:
Set the random seed for NumPy and PyTorch both to 42.

## YOUR CODE HERE
```py
np.random.seed(42)
torch.manual_seed(42)
```
## Step 3:
Create a NumPy array called arr that contains 6 random integers between 0 (inclusive) and 5 (exclusive).

## YOUR CODE HERE
```py
arr = np.random.randint(0, 5, 6)
print(arr)
```
## Step 4:
Create a tensor x from the array above.

## YOUR CODE HERE
```py
x = torch.from_numpy(arr)
print(x)
```
## Step 5:
Change the dtype of x from int32 to int64.

## YOUR CODE HERE
```py
x = x.type(torch.int64)
print(x.dtype)
```
## Step 6:
Reshape x into a 3x2 tensor.

## YOUR CODE HERE
```py
x = x.reshape(3, 2)
print(x)
```
## Step 7:
Return the right-hand column of tensor x.

## YOUR CODE HERE
```py
print(x[:, 1])
```
## Step 8:
Without changing x, return a tensor of square values of x.

## YOUR CODE HERE
```py
print(x ** 2)
```

## Step 9:
Create a tensor y with the same number of elements as x, that can be matrix-multiplied with x.

Use PyTorch directly (not NumPy) to create a tensor of random integers between 0 (inclusive) and 5 (exclusive).
## YOUR CODE HERE
```py
y = torch.randint(0, 5, (2, 3))
print(y)
```

## Step 10:
Find the matrix product of x and y.

## YOUR CODE HERE
```py
result = torch.matmul(x, y)
print(result)
```
# Output:
i) Import and set up PyTorch and NumPy. 
<img width="1246" height="237" alt="image" src="https://github.com/user-attachments/assets/1ff186aa-c382-4285-b076-edd3e3419677" />

ii) Create and manipulate tensors.
<img width="1203" height="381" alt="image" src="https://github.com/user-attachments/assets/ba814790-c079-4620-b8b8-a05f70a92c1d" />


iii) Perform matrix operations.
<img width="1116" height="430" alt="image" src="https://github.com/user-attachments/assets/d32e53df-fc24-4fb4-8e86-346fa9f3a7af" />

# Result:
Thus, the PyTorch tensor operations, including reshaping, dtype conversion, and matrix multiplication, were successfully performed using the Python program.
