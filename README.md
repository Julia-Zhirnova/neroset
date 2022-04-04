# neroset
```
def almost_double_factorial(n):
    res = 1
    for i in range(1, n+1):
        if (i%2 == 1):
            res *= i
    return res
```    
![image](https://user-images.githubusercontent.com/52165649/161512219-e9f9aeef-60c5-4d09-85f8-58492de24ca5.png)
```
sorted_items = sorted(items, key=lambda x: x[1][-1])
```
![image](https://user-images.githubusercontent.com/52165649/161517765-ff263498-e6d0-4758-9a7f-5335d7e09a21.png)
```
x[::-2] = [-1, -3, -5]
```
![image](https://user-images.githubusercontent.com/52165649/161518206-15c5ab60-93ec-4f84-b7c8-a796cfe77a50.png)

```

def cumsum_and_erase(A = [], erase = 1):
    B = []
    N = len(A)
    for i in range(0, N - 1):
        if A[i] == 1:
            A.remove(A[i])
        for i in B:
            B[0] = A[0]
            B = B[i - 1] + A[i]
    return B

A = [5, 1, 4, 5, 14]
B = cumsum_and_erase(A, erase=1)



print(cumsum_and_erase(A, erase=1))
```
