# Reema-praba-V-Module7
# 19CS301-Module7
### Register No - 212222020020
### Name - Reema praba v

# ExNo: 7.1 Recursion
### Aim: To write a Python program to find the product of first n Natural Numbersmax_speed(),change_gear() override the same methods of base class  using method overriding
### Algorithm:

**STEP 1:** Start.

**STEP 2:** Define a function `prod_num(n)` that:
- Checks if `n <= 0`, then returns 1.
- Otherwise, returns `n * prod_num(n-1)` (recursive call).

**STEP 3:** Take input `n` from the user.

**STEP 4:** Call the function `prod_num(n)` and print the result.

**STEP 5:** Stop.

### Program:
```
def prod_num(n):
    if n<=0:
       return 1
    return ((n)*prod_num(n-1))
n = int(input())
print("Result is",prod_num(n))

```
### OUTPUT:
![image](https://github.com/user-attachments/assets/d3db6c26-2d70-4d29-beeb-2dd37388ed07)

### Result: Thus, the given program is implemented and executed successfully .

# ExNo: 7.2 Types of Recursion
### Aim: To write a program program to display first n natural numbers in reverse order using tail recursion.
### Algorithm:

**STEP 1:** Start.

**STEP 2:** Define a recursive function `reverse(n, curr=1)`:
- If `curr` is greater than `n`, return (stop recursion).
- Otherwise, call `reverse(n, curr+1)` recursively.
- After the recursive call returns, print `curr` followed by a space.

**STEP 3:** Take input `n` from the user.

**STEP 4:** Call the function `reverse(n)`.

**STEP 5:** Stop.

### Program:
```
def reverse(n,curr=1):
     if n<curr:
        return
     reverse(n,curr+1)
     print(curr,end=" ") 
n =int(input())
reverse(n)

```
### OUTPUT:
![image](https://github.com/user-attachments/assets/b98ac1db-4f8d-444f-8985-71bc27955acf)
![image](https://github.com/user-attachments/assets/1c6e982f-1aa7-4989-b043-a48d0ccfa063)

### Result: Thus, the given program is implemented and executed successfully .

# ExNo: 7.3 Taylor Series
### Aim: To write a python program to evaluate the Sinh( x )  for  n terms terms  using recursion ![image](https://github.com/user-attachments/assets/396660e6-6547-4ab8-a5ce-349f1afcbd10)

### Algorithm:

**STEP 1:** Start.

**STEP 2:** Define a recursive function `fact(n)` to calculate factorial:
- If `n == 1`, return 1.
- Else, return `n * fact(n-1)`.

**STEP 3:** Define a recursive function `ser(x, n)` to calculate the series sum:
- If `n == 0`, return `x`.
- Else, return `(x^(2n+1) / fact(2n+1)) + ser(x, n-1)`.

**STEP 4:** Take input values for `x` and `n` from the user.

**STEP 5:** Call `ser(x, n)` and print the result.

**STEP 6:** Stop.

### Program:
```
import math
def ser(x,n):
    if n==0:
       return x
    else:
       return (pow(x,2*n+1)/fact(2*n+1)+ser(x,n-1))
def fact(n):
    if(n==1):
       return 1
    else:
       return n*fact(n-1)
x = int(input())
n = int(input())
print(ser(x,n))

```
### OUTPUT:
![image](https://github.com/user-attachments/assets/e6cb8259-73b3-4eda-8e2d-142cbe26c706)

### Result: Thus, the given program is implemented and executed successfully .

# ExNo: 7.4 Solve by reccurance relation
### Aim: To write a python program to count the positive numbers using recursion.349f1afcbd10)
### Algorithm:

**STEP 1:** Start.

**STEP 2:** Define a function `ispositive(num)` that:
- Returns `1` if `num > 0`.
- Otherwise, returns `0`.

**STEP 3:** Define a recursive function `totalpositive(l, n)` that:
- If `n == 0`, returns `0`.
- Otherwise, returns `ispositive(l[n-1]) + totalpositive(l, n-1)`.

**STEP 4:** Take input `n` (number of elements) from the user.

**STEP 5:** Initialize an empty list `l`.

**STEP 6:** Use a loop to take `n` integer inputs and append them to list `l`.

**STEP 7:** (Optional) Call `totalpositive(l, n)` to get the count of positive numbers.

**STEP 8:** Stop.

### Program:
```
def ispositive(num):
    #Add your code here
    return 1 if num>0 else 0
    
def totalpositive(l, n):
    #Add your code here
     if n==0:
        return 0
     return ispositive(l[n-1])+totalpositive(l,n-1)
    
n=int(input())
l=[]
for i in range(n):
    x=int(input())
    l.append(x)

```
### OUTPUT:
![image](https://github.com/user-attachments/assets/b80a53c0-3f49-481e-8e6f-479a5dfc2d62)
![image](https://github.com/user-attachments/assets/b768db01-f4f2-4fd7-87aa-81c81fd028dd)

### Result: Thus, the given program is implemented and executed successfully .
