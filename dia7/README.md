## [30-Días-de-Python](./..)

# Día 7

## Listas y Diccionarios

Hay 2 tipos de datos que no vimos hasta ahora, pero son muy usados y a partir de ahora vamos a emprezar a utlizarlos en todos los ejercicios. que son las _listas_ y _diccionarios_

### Empecemos

- ## Listas
  Las Listas son un tipo de dato que como dice el nombre es una lista de datos. Qué datos? cualquiera. veamos un ejemplo  
  para definir una lista utilizaremos corchetes o []

```python

mi_lista= []
mi_otra_lista = [2,'hola','adios',['otra','lista'],True,None]
```

Como se puede ver en el código de arriba, tenemos 2 listas, una _vacia_ y la otra con una serie de datos de diferentes tipos, cada 'dato' se separa por una coma y tambien cada dato tiene un **indice** que es la posición en la que se encuentra.

Veamos un poco mas

```python

mi_otra_lista = [2,'hola','adios',['otra','lista'],True,None]
## incides ##### 0,  1   ,    2   ,      3         , 4 , 5


"""
como vemos en el comentario debajo de la lista cada dato tiene su _incide_, este siempre arranca de 0
e identifica que posición tiene cierto 'elemento' dentro de la lista
"""

```

Ahora bien como obtengo el dato de la lista?

```python
mi_otra_lista = [2,'hola','adios',['otra','lista'],True,None]
## incides ##### 0,  1   ,    2   ,      3         , 4 , 5

"""
si quiero acceder al hola debo hacer lo siguiente
"""


print(mi_otra_lista[1])

# PODES COPIAR EL CÓDIGO Y EJECUTARLO

```

como vemos arriba, detro del print para acceder a un valor únicamente hay que escribir [] seguido del nombre de la variable que contiene la lista, y dentro de estos [indice] colocar el _indice_

```python
mi_otra_lista[indice] <-
```

**_Podes probar que pasa con un indice que no existe_**

Qué otras cosas se puede hacer con las listas?  
Bueno a las listas las podemos añadir, eliminar y modificar datos. Es una buena forma de tener muchos datos en un solo lugar.
Vamos a ver cada uno. (**_SOLO FUNCIONAN EN LISTAS_**)

```python

"""
Partiendo de una lista vacia
"""
mi_lista=[]

# Añadir

mi_lista.append('Hola')
mi_lista.append("Mundo")
"""
añade un nuevo elemento a la lista dada al final.
"""
print(mi_lista)

# Quitar el ultimo elemento
mi_otra_lista = [2,'hola','adios',['otra','lista'],True,None]
valor_quitado = mi_otra_lista.pop()
"""
El metodo pop() quita el ultimo elemento de esta, se puede especificar un indice dentro de los parentesis
y asi quitar un elemento especifico. Si se provee un indice a eliminar se reinician los inidices con
los elementos restantes.
"""
print(mi_otra_lista)
print(valor_quitado)


# Buscar indice

indice_buscado = mi_otra_lista.index('hola')
"""
En este caso nos devuelve el indice del primer elemento encontrado que concuerde con lo colocado
"""
print(indice_buscado)


```

## Sumar, Multiplicar listas

También podemos sumar,multiplicar 2 listas e incluso compararlas, veamos un ejemplo

```python
lista_1=[1,5,6]
lista_2=[7,8,9]


lista_3=lista_1 + lista_2
# resultado [1,5,6,7,8,9]


lista_4 = lista_1 * 2
# resultado [1,5,6,1,5,6]


#Comprar 2 listas

print(lista_1 == lista_2)
# imprime False


"""
NOTA:

No se pueden restar dividir, lo podes probar en tu editor de código

"""
```

## Continuemos con..

- ## Diccionarios

Los diccionarios son otro tipo de dato que al igual que las listas contiene un conjunto de datos, pero a diferencia de las listas que cada dato tiene su indice según su posición, aca cada dato tiene una 'clave', 'llave' o 'key' como se la conoce normalmente.

Veamos un poco como se compone.

```py
diccionario = {
  'clave':'valor'
}

"""
  Un diccionario tiene esta estructura, su cuerpo empieza con una llave de apertura { y termina con una llave de cierre }.

  Dentro se define cada dato, para cada uno de los datos debe existir una 'clave' o 'key', despues se ponen : que es el que asigna el valor a esa 'clave'. Despues de estos : va el valor correspondiente,
  el valor puede ser cualquier tipo de dato aceptado por python, incluso una lista u otro diccionario.

  NOTA:
  la palabra 'dict' esta reservada dentro de python.

"""
```

hay ciertas cosas que podemos hacer con los diccionarios, vamos por lo básico y lo que más se útiliza.

```python

"""
Tenemos acá un diccionario que serán datos de una persona.
Fijense como el valor puede ser cualquier tipo de dato, en cambio las 'claves' o 'key' siempre estan entre comillas, pueden ser dobles o simples.
"""

diccionario_persona={
  'nombre':'John',
  'apellido':'Doe',
  'edad':45,
  'casado':False
}



print(diccionario_persona.values())
# Nos devuelve una lista con toods los valores que hay en el diccionario
print(diccionario_persona.keys())
# Nos devuelve una lista con todas las 'claves' del diccionario
print(diccionario_persona.items())
# Nos devuelve una lista de listas(Tuplas en realidad) que en el indice 0 tiene la 'clave' y el indice 1 tiene el valor



```

> [!TIP]
> Podes ejecutar este código para ver lo que pasa

### Otras operaciones con los diccionarios

Una cosa que no vimos hasta ahora es como acceder a los datos, y se puede hacer de la siguiente manera

```python


"""
Suponiendo que tenemos el mismo diccionario, para acceder a alguno de los datos que trae podemos utilizar la clave como si fuera un indice
"""
diccionario_persona={
  'nombre':'John',
  'apellido':'Doe',
  'edad':45,
  'casado':False
}


print(diccionario_persona['nombre'])
# Mostrara el nombre de la persona en este caso 'John'

"""
Es similar a las listas, nada mas que en lugar del indice se utiliza la clave.
"""

```

#### Si queremos agregar nuevos campos podemos simplemente repetir lo siguiente:

```python

mi_diccionario={
  'nombre':'George'
}

"""
Queremos agregarle un apellido o incluso la edad
"""
print(mi_diccionario)
# imprime el diccionario de arriba


mi_diccionario["apellido"]='Johnson'
mi_diccionario['edad']=70

print(mi_diccionario)
# Imprime el diccionario modificado con los nuevos campos 'apellido' y 'edad'




```

> [!TIP]
> Ejecuta el código para ver como funciona
