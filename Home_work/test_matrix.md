Документация к модулю операции с матрицами
===
Описание класса Matrix
---
"""python
>>> from Home_work import matrix
>>> A = matrix.Matrix(2, 3)
>>> A.matrix = [[1, 2, 3], [4, 5, 6]]
>>> B = matrix.Matrix(3, 2)
>>> B.matrix = [[7, 8], [9, 10], [11, 12]]
>>> C = matrix.Matrix(2, 2)
>>> C.matrix = [[1, 2], [3, 4]]
>>> G = matrix.Matrix(2, 2)
>>> G.matrix = [[3, 4], [5, 2]]
>>> H = matrix.Matrix(2, 3)
>>> H.matrix = [[1, 2, 3], [4, 5, 6]]
>>> A == B
False
>>> C == G
False
>>> A == H
True
>>> print(C + G, end="")
4 6
8 6
>>> print(A + B)
Traceback (most recent call last):
...
ValueError: Matrices should have the same dimensions for addition.
>>> print(A * B, end="")
58 64
139 154
>>> print(A * H, end="")
Traceback (most recent call last):
...
ValueError: Number of columns in the first matrix must match the number of rows in the second matrix for multiplication.
>>> print(C * G, end="")
13 8
29 20

"""
