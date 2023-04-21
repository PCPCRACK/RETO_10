# RETO_10

Desarrollar un algoritmo que calcule el promedio de un arreglo de reales.
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
Desarrollar un algoritmo que calcule el producto punto de dos arreglos de números enteros (reales) de igual tamaño.
```python

```

Hacer un algoritmo que deje al final de un arreglo de números todos los ceros que aparezcan en dicho arreglo.
```python

```
Revisar que son los algoritmos de sorting, entender bubble-sort (enlace a implementación).
```python

```
