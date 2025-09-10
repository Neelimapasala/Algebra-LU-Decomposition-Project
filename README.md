# LU Decomposition: Applications and Advancements  

This repository contains my project on **LU Decomposition**, a fundamental matrix factorization method in numerical linear algebra. The project explores both the **mathematical principles** and **real-world applications** of LU decomposition, with a focus on **numerical weather prediction (NWP)** and **hurricane tracking**.  

## 📌 Project Overview  

- **Objective**: To study LU decomposition and analyze its computational benefits in solving large-scale systems of equations.
  
- **Methodology**:  
  - Factorization of matrix **A** into **L (Lower Triangular)** and **U (Upper Triangular)** matrices  
  - Forward and backward substitution for solving **Ax = b**  
  - Handling **sparse matrices** efficiently  
  - Real-time updates in weather models using LU decomposition
    
- **Applications**:
  - Numerical weather prediction & climate modeling  
  - Real-time hurricane tracking (Case study: **Hurricane Ian, 2022**)  
  - Engineering, physics, and data science computations  


## 🧮 Example (Python LU Decomposition)  

Here’s a simple Python example using **SciPy**:  

```python
import numpy as np
from scipy.linalg import lu

# Example matrix
A = np.array([[2, 3, 1],
              [4, 7, 7],
              [6, 18, 22]])

# LU Decomposition
P, L, U = lu(A)

print("Matrix A:\n", A)
print("\nPermutation Matrix P:\n", P)
print("\nLower Triangular Matrix L:\n", L)
print("\nUpper Triangular Matrix U:\n", U)
