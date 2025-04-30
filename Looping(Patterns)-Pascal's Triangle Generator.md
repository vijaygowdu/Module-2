## EX.NO2(E) LOOPING (PATTERNS)-PASCAL'S TRIANGLE GENERATOR 
## Aim:  
To write a Python program to generate Pascal's Triangle using numbers, where the number of rows is provided by the user.  
## Algorithm: 
Step 1: Start the program. 

Step 2: Prompt the user to input the number of rows, say num_rows. 

Step 3: Define a function factorial(n) to calculate the factorial of a number n. 

Step 4: Define a function combination(n, k) that uses the formula: 
C(n,k)=n!k!(n−k)!C(n, k) = \frac{n!}{k!(n-k)!}C(n,k)=k!(n−k)!n!  

Step 5: Loop from i = 0 to num_rows - 1 (each iteration is a row of the triangle): 

      - Step 5.1: Print spaces for formatting: 
        Print ' ' * (num_rows - i - 1) to center-align the triangle. 
      - Step 5.2: Loop from j = 0 to i (each iteration is a value in the row): 
              o Compute the value using the combination formula C(i, j). 
              o Print the value with a space. 
      - Step 5.3: Move to the next line. 

Step 6: End the program. 
## PROGRAM:  
```
def factorial(n): 
  if n == 0 or n == 1: 
     return 1 
   return n * factorial(n - 1) 
def combination(n, k): 
   return factorial(n) // (factorial(k) * factorial(n - k)) 
# Step 2: Input from user 
num_rows = int(input())

# Step 5: Generate Pascal's Triangle 
for i in range(num_rows):

  # Step 5.1: Print spaces 
   print(' ' * (num_rows - i - 1), end='') 
  # Step 5.2: Print values in the row 
   for j in range(i + 1): 
      print(combination(i, j), end=' ') 
  # Step 5.3: Move to next line 
  print()
```
## OUTPUT: 
![image](https://github.com/user-attachments/assets/ce01ea1f-3e5a-4cb6-8782-0f582ad7e0f5)
## RESULT:  
Thus, the program has been successfully executed 
