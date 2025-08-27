import numpy as np

#crear arreglos

arr = np.array([1,2,3,4])
print(arr)

arr2 = np.array([[1,2,3], [4,5,6]])
print(arr2)

#Reshape

arr = np.arange(6).reshape(2,3)
print(arr)

#concatenar

a = np.array([[1,2,3],[4,5,6]])
b = np.array([[3,5,7],[2,4,6]])

arr = np.concatenate ([a,b], axis=0)
print(arr)
arr2 = np.concatenate ([a,b], axis=1)
print(arr2)

#operaciones basicas

a = np.array ([1,2,3,4])
b = np.array ([5,6,7,8])

arr = np.add (a,b)
print(arr)
arr2 = np.subtract (b,a)
print(arr2)
arr3 = np.multiply (a,b)
print(arr3)
arr4 = np.divide (a,b)
print(arr4)