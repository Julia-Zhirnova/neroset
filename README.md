# neroset
Почти двойной факториал
```
def almost_double_factorial(n):
    res = 1
    for i in range(1, n+1):
        if (i%2 == 1):
            res *= i
    return res
```    
Хитрая сортировка
```
sorted_items = sorted(items, key=lambda x: x[1][-1])
```
Слайсы
```
x[::-2] = [-1, -3, -5]
```
Создание массивов
```
def cumsum_and_erase(A = [], erase = 1):
    B = []
    C = []
    N = len(A)
    B.append(A[0])
   
    for i in range(1, N):
        B.append(A[i]+B[i-1])
    i=0
    while i<N:
        if B[i] != erase:
            C.append(B[i])
        i= i+1
    
    return C
```
