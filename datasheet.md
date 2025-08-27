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

#estadisticas

a = np.array ([1,2,3,4,5,6,7,8,9])

arr = np.mean(a)
print(arr)
arr2 = np.std(a)
print(arr2)
arr3 = np.sum(a)
print(arr3)
arr4 = np.max(a)
print(arr4)
arr5 = np.min(a)
print(arr5)

#secuencias

rango = np.arange(0,10,2)
print(rango)
linea = np.linspace(0,1,5)
print(linea)

#aleatorio

np.random.seed(42)

aleatorio_uniforme = np.random.rand(2, 2)
print(aleatorio_uniforme)
aleatorio_normal = np.random.randn(2, 2)
print(aleatorio_normal)
aleatorio_enteros = np.random.randint(0, 10, (2, 2))
print(aleatorio_enteros)

#algebre lineal

a = np.array([[1,2], [3,4]])

inversa = np.linalg.inv(a)
print(inversa)
determinante = np.linalg.det(a)
print(determinante)
vectores_propios = np.linalg.eig(a)
print(vectores_propios)
solucion = np.linalg.solve(a, np.array([5, 6]))
print(solucion)

import pandas as pd

data = {
    'Nombre': ['Ana', 'Luis', 'Carlos'],
    'Edad': [23, 31, 29],
    'Ciudad': ['Bogotá', 'Medellín', 'Cali']
}

df = pd.DataFrame(data)
print(df)

