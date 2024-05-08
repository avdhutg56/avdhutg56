#Program for Descartes sign rule
a=[]
b=[]
proots=0
nroots=0
croots=0
print('f(x)=x^3-3x^2+2x-1')
coeff=input('Enter polynomial coefficients separated by space:')
a=list(map(float,coeff.split()))
for j in range (0,len(a)-1):
 if a[j]*a[j+1]<0:
    proots=proots+1
for j in range(0,len(a)):
    b.append(a[j]*((-1)**j))
for j in range (0,len(a)-1):
 if b[j]*b[j+1]<0:
    nroots=nroots+1
    croots=len(a)-1-proots-nroots
print("\n applying Descartes rule of signs , we get")
print("no of +ve real roots:atmost",proots)
print("no of -ve real roots:atmost",nroots)
print("no of complex roots:atleast",croots)
Result:

f(x)=x^3-3x^2+2x-1
Enter polynomial coefficients separated by space:1 -3 2 -1

 applying Descartes rule of signs , we get
no of +ve real roots:atmost 3
no of -ve real roots:atmost 0
no of complex roots:atleast 0




#2D array formation 
import numpy as np
#input section matrix
M1 = np.array([[1,4],[5,6]])
M2 = np.array([[1,-4],[3,-2]])
#output section matrix
#Matrix Addition 
print("[M1]+[m2]=",M1+M2)
#Matrix Substraction
print("[M1]-[m2]=",M1-M2)
#Matrix Multiplication
print("[M1][m2]=",M1.dot(M2))
#Matrix Transpose
print("Transpose of [M1]=",M1.transpose())

[M1]+[m2]= [[2 0]
 [8 4]]
[M1]-[m2]= [[0 8]
 [2 8]]
[M1][m2]= [[ 13 -12]
 [ 23 -32]]
Transpose of [M1]= [[1 5]
 [4 6]]

