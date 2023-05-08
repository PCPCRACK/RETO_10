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
# De librerias importa la funcion coseno
from math import cos 
  
if __name__ == "__main__":

    # Pide la cantidad de numeros en la lista
    num = int(input("tamaño del arreglo: "))

    # Define la cantidad de vectores igual a 2
    vect = int(2)

    # lista vacia
    b = []

    # Establece un contador
    sum = float(1)

    # Define dios igual a 2
    dios = int(2)

    # Define ayuda igual a 0
    ayuda = float(0)

    # Define teta el cual es el angulo entre los vectores
    teta = float(input("algulo entre los dos vectores: "))

    # Establece un ciclo del tamaño del los vectores
    for j in range(vect):

        # Crea una lista vacia
        a = []

        # Establece un ciclo del tamaño del arreglo
        for i in range(num):

            # Establece n como el numero ingresado
            n = float(input(f"lista del vector {j+1}, dato N° {i+1}: "))

            # Vuelve n un numero absoluto
            n = abs(n)

            # Lo añade a a lista a
            a.append(n)

        # al acabar el ciclo guarda la lista a en la lista b    
        b.append(a)

    # Establece un ciclo del tamaño de la lista b
    for i in range(len(b)):

        # Imprime el valor de b en la lista
        print(b[i])

    # Establece un ciclo del tamaño del arreglo
    for j in range(num):

        # Establece un ciclo del tamaño de la lista b
        for fila in b:

            # Si la dividion por producto de dios es igual a cero
            if dios%2 == 0:

                # El valor de la fila[j] se suma al valor de ayuda
                ayuda += fila[j]

            # sum se multiplica por el valor de fila[j] 
            sum *= fila[j]

            # dios se añade un valor
            dios += 1

        # Se imprime el producto punto de los vectores
        print(f"el producto punto de los vectores {1} numero {j+1} y {2} numero {j+1} son (|{ayuda} x {fila[j]}| x cos) = {sum*cos(teta)}")

        # Se imprime el valor de sum
        print(sum)

        # sum toma el valor de igual a 1
        sum = 1

        # ayuda toma el valor de igual a 0
        ayuda = 0

        # dios toma el valor de igual a 2
        dios = 2
```
```python
# De librerias importa la funcion coseno
from math import cos 
  
if __name__ == "__main__":

    # Pide la cantidad de numeros en la lista
    num = int(input("tamaño del arreglo: "))

    # Define la cantidad de vectores igual a 2
    vect = int(2)

    # lista vacia
    b = []

    # Establece un contador
    sum = float(1)

    # Define dios igual a 2
    dios = int(2)

    # Define ayuda igual a 0
    ayuda = float(0)

    # Define teta el cual es el angulo entre los vectores
    teta = float(input("algulo entre los dos vectores: "))

    # Define un contador
    trikitrakelas = float(0)

    # Establece un ciclo del tamaño del los vectores
    for j in range(vect):

        # Crea una lista vacia
        a = []

        # Establece un ciclo del tamaño del arreglo
        for i in range(num):

            # Establece n como el numero ingresado
            n = float(input(f"lista del vector {j+1}, dato N° {i+1}: "))

            # Lo añade a a lista a
            a.append(n)

        # al acabar el ciclo guarda la lista a en la lista b    
        b.append(a)

    # Establece un ciclo del tamaño de la lista b
    for i in range(len(b)):

        # Imprime el valor de b en la lista
        print(b[i])

    # Establece un ciclo del tamaño del arreglo
    for j in range(num):

        # Establece un ciclo del tamaño de la lista b
        for fila in b:

            # Si la dividion por producto de dios es igual a cero
            if dios%2 == 0:

                # El valor de la fila[j] se suma al valor de ayuda
                ayuda += fila[j]

            # sum se multiplica por el valor de fila[j] 
            sum *= fila[j]

            # dios se añade un valor
            dios += 1

        # Se añade el valor de sum antes de que retorne a 1
        trikitrakelas += sum

        # sum toma el valor de igual a 1
        sum = 1

        # ayuda toma el valor de igual a 0
        ayuda = 0

        # dios toma el valor de igual a 2
        dios = 2
        
    # Se imprime el producto punto de los vectores
    print(f"el producto punto de los vectores {1} y {2} es {trikitrakelas}")
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
