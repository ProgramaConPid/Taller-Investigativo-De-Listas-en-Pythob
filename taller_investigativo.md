# TALLER INVESTIGATIVO DE ARRAYS EN PYTHON

# 1. ¿Qué es un array o lista en Python?

* >Investiga qué son los arrays (o listas) en Python y para qué se utilizan.

R/= Son estructuras de datos versatiles que permiten almacenar una coleccion ordenada de elementos

* >¿Cómo se declara una lista vacía?

R/= mi_lista = []

* >¿Cómo se crea una lista con valores iniciales?

R/= mi_lista = ["valor1", "valor2", "valor3"]

### EJEMPLO PRACTICO ![alt text](imgs/image-1.png)

* Crea una lista llamada mi_lista con los números del 1 al 5.

```python

mi_lista = [1, 2, 3, 4, 5]

```

---

# 2. ¿Cómo accedemos a los elementos de una lista?

* >¿Cómo se accede al primer elemento de una lista?

R/= En los arrays y/o listas el primer indice de este generalmente es el 0 por lo tanto:

Array -> mi_array = ["hola", "pepe"] - Acceder primer elemento &larr; print(mi_array[0]) 

La ejecucion imprimiria &larr; "hola"

* >¿Qué significa usar un índice negativo?

R/= Los indices negativos permiten acceder a los elementos desde el final de una lista, es decir: la posicion [-1] seria el ultimo elemento, la posicion [-2] seria el elemento anterior al ultimo y asi sucesivamente.

* >¿Qué pasa si intento acceder a un índice que no existe?

R/= Al intentar acceder a un indice inexistente de una lista, python arrojara un error diciendo que el indice de la lista esta fuera del rango.

## EJEMPLO PRACTICO ![alt text](imgs/image-1.png)

* Crea una lista [10, 20, 30, 40] y muestra el primer y el último elemento.

```python

mi_lista = [10, 20, 30, 40]

# Primer elemento
print(mi_lista[0]) # Imprime 10

# Ultimo elemento
print(mi_lista[-1]) # Imprime 40

```

---

# 3. ¿Qué es el "slicing" o rebanado de listas?

* >¿Qué significa "slicing" en listas?

R/= es una forma de extraer una subsección de una secuencia (como una lista, tupla o cadena) utilizando una sintaxis específica, la sintaxis es la siguiente &larr; [start:stop:step]

* >¿Cómo se obtiene una sublista usando slicing?

### EN CODIGO &#8595;

```python

# Obtener una sublista usando slicing
mi_lista = [1, 2, 3, 4, 5, 6]

# Obtener los elementos 1, 2, 3, 4
print(mi_lista[0:4]) # Imprime 1, 2, 3, 4

```

* >¿Qué significa dejar vacío el inicio o el final en el slicing?

R/= Al dejar vacio el inicio en el slicing este asumira el indice 0, es decir que empezara por el primer elemento y al dejar vacio el final en el slicing este asumira el valor -1, es decir el indice final de la lista.

### EN CODIGO &#8595;

```python

mi_lista = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

# Primer espacio del slicing vacio
print(mi_lista[:5]) # Imprimira desde el indice 0 hasta el 5

# Ultimo espacio del slicing vacio
print(mi_lista[7:]) # Imprimira desde el indice 7 hasta el 10

```

## EJEMPLO PRACTICO ![alt text](imgs/image-1.png)

- A partir de [10, 20, 30, 40, 50], obtén:

* Los elementos del índice 1 al 3.
* Los primeros 3 elementos.
* Los elementos desde el índice 2 hasta el final.

```python

# Lista
mi_lista = [10, 20, 30, 40, 50]

# Obtener elementos del indice 1 al 3
print(mi_lista[1:3]) # Imprimira 20, 30, 40

# Obtener los primeros tres elementos
print(mi_lista[:2]) # Imprimira 10, 20, 30

# Obtener los elementos desde el indice 2 hasta el final 
print(mi_lista[2:]) # Imprimira 30, 40, 50

```

---

# 4. ¿Cómo modificamos los elementos de una lista?

* >¿Cómo se cambia el valor de un elemento de la lista?

R/= El valor de un elemento en un arreglo se cambia de la siguiente manera:

```python

# Cambiar el elemento del indice 3 por el valor 99
mi_lista[3] = 99

```

* >¿Qué pasa si modificamos un índice que no existe?

R/= Al intentar modificar un indice que no existe, python arrojara un error similiar al de intentar acceder a un indice que no existe, el error que muestra es: asignamiento de indice fuera de rango.

## EJEMPLO PRACTICO ![alt text](imgs/image-1.png)

* Cambia el tercer elemento de [10, 20, 30, 40] por 99.

```python

# Lista
mi_lista = [10, 20, 30, 40]

# Modificar el tercer elemento por el valor 99
mi_lista[2] = 99

# Imprimir la lista
print(mi_lista) # Imprimira [10, 20, 99, 40]

```

---

# 5. ¿Cómo agregamos nuevos elementos a una lista?

* >¿Cómo se agrega un elemento al final de la lista?

R/= Para agregar un elemento al final de una lista se utiliza el metodo .append(elemento)

## EN CODIGO &#8595;

```python

# Lista 
mi_lista = [10, 20, 30, 40]

# Agregar el valor 50 al final de la lista
mi_lista.append(50)

# Imprimir lista
print(mi_lista) # Imprimira [10, 20, 30, 40, 50]

```

* >¿Cómo se inserta un elemento en una posición específica?

R/= Para insertar un elemento en un indice especifico de una lista se usa el metodo .insert(indice, nuevo_elemento)

## EN CODIGO &#8595;

```python

# Lista
mi_lista = [2, 4, 6, 8, 10]

# Insertar el elemento 5 en el indice 2
mi_lista.insert(2, 5)

# Imprimir la lista
print(mi_lista) # Imprimira [2, 4, 5, 6, 8, 10]

```

* >¿Cómo se combinan dos listas en una sola?

R/= Para combinar dos listas en una sola lista se usa el metodo .extend(lista_a_unir).

## EN CODIGO &#8595;

```python

# Lista
lista1 = [1, 2, 3, 4, 5]
lista2 = [6, 7, 8, 9, 10]

# Combinar lista1 y lista2 en una sola lista
lista1.extend(lista2)

# Imprimir lista1
print(lista1) # Imprimira [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

```

## Ejemplo práctico ![alt text](imgs/image-1.png)

- A una lista [10, 20, 30] agrega:
    * El número 40 al final.
    * El número 15 en la posición 1.
    * Los números 50 y 60 al final de la lista.

```python

# Lista
mi_lista = [10, 20, 30]

# Agregar el valor 40 al final de la lista
mi_lista.append(40)

# Agregar el valor 15 en la posicion 1
mi_lista.insert(1, 15)

# Agregar el valor 50 y 60 al final de la lista
mi_lista.append(50)
mi_lista.append(60)

# Imprimir la lista
print(mi_lista) # Imprimira [10, 15, 20, 30, 40, 50, 60]

```

---

# 6. ¿Cómo eliminamos elementos de una lista?

* >¿Cómo se elimina un valor específico de una lista?

R/= Para eliminar un valor especifico de una lista se usa el metodo .remove(valor)

### EN CODIGO &#8595;

```python

# Lista
mi_lista = [3, 6, 9, 12]

# Eliminar el valor 9 de la lista
mi_lista.remove(9)

# Imprimir lista
print(mi_lista) # Imprimira [3, 6, 12]

```

* >¿Qué hace el método pop()?

R/= El metodo pop() si no se le pasa un indice eliminara el ultimo elemento de la lista

### EN CODIGO &#8595;

```python

# Lista
mi_lista = [1, 2, 3]

# Eliminar el ultimo elemento de la lista con el metodo .pop()
mi_lista.pop()

# Imprimir lista


```

* >¿Cómo se elimina un elemento usando del?

## EJEMPLO PRACTICO ![alt text](imgs/image-1.png)

- De la lista [10, 20, 30, 40, 50], realiza las siguientes acciones:
    * Elimina el número 30.
    * Elimina el último elemento.
    * Elimina el segundo elemento (índice 1).

```python

# Lista
mi_lista = [10, 20, 30, 40, 50]

# Eliminar el numero 30
mi_lista.remove(30)

# Eliminar el ultimo elemento
mi_lista.pop()

# Eliminar el segundo elemento (indice 1)
mi_lista.del(1)

```

---

# 7. ¿Cómo buscamos elementos dentro de una lista?

* >¿Cómo se verifica si un elemento está presente en una lista?

R/= Para verificar si un elemento, cadena o valor se encuentra en una lista, se pueda el operador in.

### EN CODIGO &#8595;

```python

# Lista
mi_lista = ["Hola", "Pepe", "Carlos"]

# Verificar si "Pepe" se encuentra en mi_lista
print("Pepe" in mi_lista) # True

```

* >¿Cómo encontrar el índice de un elemento?

R/= Para encontrar el indice de un elemento en una lista, se usa el metodo index(valor)

### EN CODIGO &#8595;

```python

# Lista
mi_lista = ["Hola", "Pepe", "Carlos"]

# Encontrar el indice de "Carlos"
print(mi_lista.index("Carlos")) # Indice 2

```

* >¿Cómo contar cuántas veces aparece un valor en la lista?

R/= Para contar cuantas veces se repite un elemento en una lista se usa el metodo .count(elemento)

### EN CODIGO &#8595;

```python

# Lista
mi_lista = ["Hola", "Pepe", "Carlos"]

# Encontrar el indice de "Carlos"
print(mi_lista.index("Carlos")) # Indice 2

```

## EJEMPLO PRACTICO ![alt text](imgs/image-1.png)

- Con la lista [10, 20, 30, 40, 50]:
    * Verifica si el número 20 está en la lista.
    * Encuentra el índice del número 30.
    * Cuenta cuántas veces aparece el número 20.

