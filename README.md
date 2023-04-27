# RETO_10

1.Desarrollar un algoritmo que calcule el promedio de un arreglo de reales.
```python
def promedio():
    
    """
    Función que solicita al usuario que ingrese los elementos de un arreglo de números reales,
    calcula el promedio de los elementos y lo devuelve como un número real.
    """

    # Inicializamos un arreglo vacío para almacenar los elementos ingresados por el usuario
    lista = []

    # Solicitamos la cantidad de elementos
    n = int(input("Ingrese la cantidad de elementos del arreglo: "))

    # Iteramos n veces para solicitar cada uno de los elementos
    for i in range(n):

        # Solicitamos el elemento i+1
        elemento = float(input(f"Ingrese el elemento {i+1}: "))

        # Agregamos el elemento ingresado al arreglo
        lista.append(elemento)

    # Calculamos la suma de los elementos del arreglo usando la función sum
    suma = sum(lista)

    # Calculamos el promedio dividiendo la suma entre la cantidad de elementos del arreglo
    return suma / len(lista)  

if __name__ == "__main__":

    #llamaremos una funcion a la cual le daremos los argumentos
    promedio = promedio()

    #imprimimos el resultado
    print(f"El promedio del arreglo es {promedio}")
```



## PD: Casi me da una embolia haciendo código el primer codigo, no daba ya me iba a dar un ataque.


2.Desarrollar un algoritmo que calcule el producto punto de dos arreglos de números enteros (reales) de igual tamaño.
```python
from math import cos
  

if __name__ == "__main__":
    num = int(input("tamaño del arreglo: "))
    vect = int(2)
    b = []
    sum = float(1)
    dios = int(2)
    ayuda = float(0)
    teta = float(input("algulo entre los dos vectores: "))
    for j in range(vect):
        a = []
        for i in range(num):
            n = float(input(f"lista del vector {j+1}, dato N° {i+1}: "))
            n = abs(n)
            a.append(n)
        b.append(a)
    for i in range(len(b)):
        print(b[i])
    for j in range(num):
        for fila in b:
            if dios%2 == 0:
                ayuda += fila[j]
            sum *= fila[j]
            dios += 1

                
        print(f"el producto punto de los vectores {1} numero {j+1} y {2} numero {j+1} son (|{ayuda} x {fila[j]}| x cos) = {sum*cos(teta)}")
        print(sum)
        sum = 1
        ayuda = 0
        dios = 2
```

3.Hacer un algoritmo que deje al final de un arreglo de números todos los ceros que aparezcan en dicho arreglo.
```python
if __name__ == "__main__":

    # Inicializamos un arreglo vacío para almacenar los elementos ingresados por el usuario
    lista = []

    # Solicitamos la cantidad de elementos
    n = int(input("Ingrese la cantidad de elementos del arreglo: "))

    # Iteramos n veces para solicitar cada uno de los elementos
    for i in range(n):

        # Solicitamos el elemento i+1
        elemento = float(input(f"Ingrese el elemento {i+1}: "))

        # Agregamos el elemento ingresado al arreglo
        lista.append(elemento)

    # estable el contador a con valor de la cantidad numero de ceros
    a = lista.index(0)

    # mientra a sea menor a -1
    while a > -1:

        # remueve el numero 0
        lista.remove(0)

        # agrega el numero cero al final de la lista
        lista.append(0)

        # resta 1 al contador
        a -= 1

    # imprimimos el resultado
    print(lista)
```
Revisar que son los algoritmos de *sorting*, entender *bubble-sort* ([enlace](https://www.geeksforgeeks.org/bubble-sort/) a implementación).
