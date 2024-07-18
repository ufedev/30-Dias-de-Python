## [30-Días-de-Python](./..)

# Día 8

## Bucles

Los bucles son formas de ejecutar una porción de código tantas veces como queramos o mientras se cumpla cierta condición al igual que el tema de condicionales (if elif else).  
En python tenemos varias formas de utilizar un bucle pero lo mas común es utilizar _while_ y _for_  
En este capitulo vamos a ver como funcionan ambos.

## Bucle while

while es el buble más común y simple de usar.

```python

while condicion:
    código

```

La estructura que tiene es bastante sencilla, siempre tiene una condición, mientras esta sea verdadera se seguira ejecutando el código.

> [!NOTE]
> Hay que recordar que python es un lenguaje que no usa llaves sino sangrias o tabulaciones, por eso para que consideremos al código dentro del bucle tiene que tener una tabulación o sangria de 4 espacios, si esta a la misma nivel que la palabra reservada while estara fuera del bucle

```python

numero = 0

while numero <10: # error bucle sin contenido
print(numero)     # error sin sangria
numero=numero+1   # error sin sangria

```

> [!WARNING]
> ESTE CÓDIGO NO FUNCIONA YA QUE NO RESPETA LAS SANGRIAS, aparte dará error porque el contenido del 'while' es núlo.

Veamos un ejemplo que si funciona

```python

numero = 0 # Definimos una variable

while numero<10: # Definimos la condición, en este caso mientras sea menor a 10 ejecutamos el bucle
    print(numero) # Imprimimos el número

    numero = numero + 1 # Al número por cada ciclo o iteración se le suma 1

```

> [!TIP]
> Podes copiar el código y probarlo en tu editor

## Bucle for

Este bucle es el más utilizado y super potente, abstrae muchas cosas en comparación a while.  
Para este bucle tambien vamos a aprender la palabra reservada 'range'

#### range

'range' es una palabra reservada que define un rango, es normal verla usar con for. Veamos un ejemplo con for y range

```python

for numero in range(1,10):
    print(numero)
# La estructura de for tiene el siguiente formato y lo podemos leer asi
"""
para 'el numero' en 'el rango de 1 a 10':
    imprimir('el numero')
"""

```

> [!NOTE]
> range crea un rango de un número de inicio, si no se define es 0 hasta un número final, pero este número final no se incluye, osea digamos que si ponemos range(1,10) va a ir del 1 hasta el 9. Además si ponemos un solo número en range este se considera el final y el número de inicio por defecto es 0 por ejemplo range(10) este va en el rango de 0 a 9 ya que el 10 no se incluye al ser el ultimo

Lo que tiene de potente for es que podemos recorrer listas y diccionarios facilmente. Veamos un ejemplo

```python

lista= [1,8,5,6,7,2,3]
diccionario={
    'marca':'Renault',
    'modelo':'Logan',
    'año':'2020'
}


for item in lista:
    print(item)
"""
podemos leerlo de la siguiente forma

para "cada item" en 'la lista':
    imprimir('cada item')

Una nota aparte, el nombre de 'item' puede ser cualquier otra cosa, esto es solo una variable que maneja for, pueden ponerle 'numero','dato','etc'

"""


for valor in diccionario.values(): # recorda la forma para obtener la lista de valores de los diccionarios
    print(valor)


"""
Lo podemos leer de la siguinte forma

para 'cada valor' en 'los valores del diccionario':
    imprimir('cada valor')


"""


```

> [!TIP]
> Copia el código y probalo en tu editor.

## Ya conocimos bastante sobre bucles, ahora vamos a hacer 2 ejecicios sencillos 😨

- Dada la lista 'lista_ejercicio' contar la cantidad de veces que aparece el 48 utilizando for y while

> [!NOTE]
> No lo vimos pero acá lo podemos ver, existe una palabra reservada llamada 'len' que es para saber la longitud de un texto contando los caracteres y espacios en blanco o la cantidad de elementos en un lista.

```python

lista = [2,8,3,6,7]
longitud = len(lista)

print(longitud) # 5

```

> [!NOTE]
> Recorda que las listas el primer indice siempre es el 0. osea en esta lista que esta arriba el indice 0 tiene el valor 2

#### Ejercicio

```python

lista_ejercicio= [43,13,32,44,29, 26, 18, 49, 30, 34, 29, 43, 41, 25, 38, 45, 35, 34, 49, 45, 45, 5, 43, 6, 21, 2,39, 28, 20, 43, 20, 29, 24, 28, 34, 47, 45, 16, 38, 38, 32, 34, 48, 8, 48, 34, 22, 26, 24, 18, 21, 21, 40, 41, 12, 38, 34, 43, 29, 20, 3, 17, 2, 45, 8, 23, 12, 39, 35, 33, 44, 35, 12, 43, 28, 17, 42, 50, 19, 43, 9, 26, 1, 34, 21, 26, 31, 15, 49, 50, 42, 15, 27, 6, 42, 29, 1, 42, 6, 19]

```

## Felicidades por llegar al día 8 🥳
