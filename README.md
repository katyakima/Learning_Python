# Матрицы

**Распечатать матрицу**

Используйте функцию print_matrix() для вывода квадратной матрицы размерности n:
```python
def print_matrix(matrix, n, width=1):
    for r in range(n):
        for c in range(n):
            print(str(matrix[r][c]).ljust(width), end=' ')
        print()
```

**Считать матрицу** 

Для считывания матрицы из n строк, заполненной числами, удобно использовать следующий код:
```python
n = int(input())
matrix = []
for i in range(n):
    temp = [int(num) for num in input().split()]
    matrix.append(temp)
```
**Еще примеры**
```python
def print_matrix(matrix, n, width=1):
    for r in range(n):
        for c in range(n):
            print(str(matrix[r][c]).ljust(width), end=' ')
        print()
```
Предлагаю уменьшить число параметров функции, убрав размерность (причем применимую только для квадратной матрицы) и сделать функцию универсальной, принимающей не только квадратные матрицы:
```python
def new_print_matrix(matrix, width=1):
    for r in range(len(matrix)):
        for c in range(len(matrix[0])):
            print(str(matrix[r][c]).ljust(width), end=' ')
        print()
```
Так же намного удобнее и не надо думать ни о чем)
