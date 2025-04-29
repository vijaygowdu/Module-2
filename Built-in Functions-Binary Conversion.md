
## EX.NO:2(A)	ITERATIVE STATEMENTS: PALINDROME NUMBER CHECKER


## AIM:
To write a program in python to compute whether the given number is a palindrome
## ALGORITHM:
Step1: get input and assign it to a temp variable 

Step2: iterate the input until temp>0.

Step3: give the condition of rev=(10*rev)+temp%10 and temp//=10

Step4: if rev==num then the number is a palindrome

Step5: else the number is not a palindrome

## PROGRAM:
```
num=int(input()) rev=0 temp=num while temp>0:
rev=(10*rev)+temp%10 temp//=10
if rev==num:
print("The given number {} is a Palindrome".format(num)) else:
print("The given number {} is not a palindrome".format(num))
```
## OUTPUT:

![image](https://github.com/user-attachments/assets/49e0ec16-12c3-44d2-a211-1e2be94fe3f0)






## RESULT:

Thus, the program has been successfully executed
