# Let-s-test-your-Python-skills-
Some exercices to test your python skills
Let's test your Python skills! 
Question 1 

Question: Write a program which will find all such numbers which are divisible by 7 but are not a multiple of 5, between 2000 and 3200 (both included). The numbers obtained should be printed in a sequence on a single line.

Hints: Consider use range(#begin, #end) method 
 

Question 2 Question: Write a program which can compute the factorial of a given numbers. The results should be printed in a sequence on a single line. Suppose the following input is supplied to the program: 8 Then, the output should be: 40320 

Hints: In case of input data being supplied to the question, it should be assumed to be a console input. 

Question 3 

Question: With a given integral number n, write a program to generate a dictionary that contains (i, i*i) such that is an integral number between 1 and n (both included). and then the program should print the dictionary. Suppose the following input is supplied to the program: 8 Then, the output should be: {1: 1, 2: 4, 3: 9, 4: 16, 5: 25, 6: 36, 7: 49, 8: 64} 

 

Hints: In case of input data being supplied to the question, it should be assumed to be a console input. Consider use dict()
 

Question 4 

Given a non-empty string and an int n, return a new string where the char at index n has been removed. The value of n will be a valid index of a char in the original string (i.e. n will be in the range 0..len(str)-1 inclusive). 

missing_char('kitten', 1) → 'ktten' 

missing_char('kitten', 0) → 'itten' 

missing_char('kitten', 4) → 'kittn' 

Question 5 

Write a NumPy program to convert a NumPy array into a Python list structure.

Expected Output: 

Original array elements: [[0 1] [2 3] [4 5]] 

Array to list: [[0, 1], [2, 3], [4, 5]] 
 

Question 6

Write a NumPy program to compute the covariance matrix of two given arrays. 

Original array1: [0 1 2] 

Original array2: [2 1 0] 

Covariance matrix of the said arrays: [[ 1. -1.] [-1. 1.]]
 

Question 7

Question: Write a program that calculates and prints the value according to the given formula: Q = Square root of [(2 * C * D)/H] Following are the fixed values of C and H: C is 50. H is 30. D is the variable whose values should be input to your program in a comma-separated sequence. Example Let us assume the following comma separated input sequence is given to the program: 100,150,180 The output of the program should be: 18,22,24 

Hints: If the output received is in decimal form, it should be rounded off to its nearest value (for example, if the output received is 26.0, it should be printed as 26) In case of input data being supplied to the question, it should be assumed to be a console input. 

***CORRECTION***
Question 1
x=0
for i in range(2000,3201):
    if i%7==0 and (i/5)!=0:
        x+=i
print(x)    

Question 2
n =8
fact = 1
  
for i in range(1,n+1): 
    fact = fact * i 
      
print ("The factorial of n is : ") 
print (fact)
The factorial of n is : 
40320

Question 3
x = int(input())
d = {}
for i in range(1,x+1):
        d[i]=i*i
print(d)
3
{1: 1, 2: 4, 3: 9}

Question 4
def missing_char(str,n):
    return str[:n]+str[n+1:]
missing_char('he llo',3)
'he lo'
Question 5
import numpy as np
​
a=np.array(((0,1),(2,3),(4,5)))
l = a.tolist()
print(l)
​
[[0, 1], [2, 3], [4, 5]]

Question 6
import numpy as np
Tab1 =np.array ([0,1,2]) 
​
Tab2 =np.array([2,1,0]) 
X = np.array([Tab1,Tab2 ])
​
cov = np.cov(X,bias=True)
print (cov)
[[ 0.66666667 -0.66666667]
 [-0.66666667  0.66666667]]
 
Question 7
C=50 
x=[]
H=30
ch=input()
x=ch.split(',')
for i in x:
    D=int(x[i])
    Q=sqrt([(2 * C * D) / H] )
    
print(Q)
 





C=50 
x=[]
H=30
ch=input()
x=ch.split(',')
for i in x:
    D=int(x[i])
    Q=sqrt([(2 * C * D) / H] )
    
print(Q)
