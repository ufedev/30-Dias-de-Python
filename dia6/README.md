## [30-Días-de-Python](./..)

# Día 6

## Condicionales

Los condicionales son formas de hacer que algo ocurra cuando se cumple una condición dada por nosotros.

Por ejemplo dejar pasar a un evento solo a personas mayores a 18 años, si no tiene 18 o más no pasa.

### Para este caso vamos a ver primero los operadores de condición

```py
== igual que
> mayor que
< menor que
>= mayor o igual que
<= menor o igual que
not o != distinto

and y or ( serian 'y' y 'no')
```

Cuando esta el 'and' ambas condiciones deben cumplirse  
Cuando esta el 'or' una de las 2 que se cumpla ya alcanza

Ahora para aplicar estos operadores de condición solo hace falta realizar la comparación entre 2 valores.

Hay que recordar que el resultado que dan estos operadores siempre serán valores del tipo **Booleano**,osea, que pueden ser o **_True_** o **_False_**

veamos un ejemplo a continuación

_Podes copiar el código y ejecutarlo_

```python

valor_1=int(input('Ingresa un número cualquiera sin coma y sin punto: '))
valor_2=int(input('Ingresa otro número cualquiera sin coma y sin punto: '))

print(f"los valores son iguales? {valor_1 == valor_2}")
print(f"los valores son diferentes? {valor_1 != valor_2}")
print(f"el valor 1 es mayor al valor 2? {valor_1>valor_2}")
print(f"el valor 1 es menor al valor 2? {valor_1<valor_2}")
print(f"el valor 1 es menor al valor 2 y es mayor a 5? {valor_1<valor_2 and valor_1>5}")
print(f"el valor 1 es menor al valor 2 o es mayor a 5? {valor_1<valor_2 or valor_1>5}")
# el último ejemplo solo es para mostar con el 'and' y el 'or'

"""
En caso de no ingresar números la función int() que provee python
no podra hacer la conversión de tipo de dato y dara un error
finalizanzo el programa subitamente.

"""
```

Nos daria el siguiente resultado si ambos son 10

```bash
Ingresa un número cualquiera sin coma y sin punto: 10
Ingresa otro número cualquiera sin coma y sin punto: 10
los valores son iguales? True
los valores son diferentes? False
el valor 1 es mayor al valor 2? False
el valor 1 es menor al valor 2? False
el valor 1 es menor al valor 2 y es mayor a 5? False
el valor 1 es menor al valor 2 o es mayor a 5? True
```

Existen también un par de palabras reservadas(En todos los lenguajes existen) que sirven para ejecutar una porción de código si ocurre algo y sino.

Estas palabras son _if_(si), _elif_(sino si) y _else_(sino), veamos como se aplican

_Primero una aclaración, if es el único obligatorio, elif y else son opcionales, ahora lo vemos_

**Ejemplo IF**

```python
valor_1=int(input('Ingresa un número cualquiera sin coma y sin punto: '))
valor_2=int(input('Ingresa otro número cualquiera sin coma y sin punto: '))
if valor_1==valor_2:
    print('este código se ejecuta porque se cumplio la condición, en este caso que ambos sean iguales..')

print('fin del código')
```

**Ejemplo IF y ELSE**

```python
valor_1=int(input('Ingresa un número cualquiera sin coma y sin punto: '))
valor_2=int(input('Ingresa otro número cualquiera sin coma y sin punto: '))
if valor_1==valor_2:
    print('este código se ejecuta porque se cumplio la condición, en este caso que ambos sean iguales..')
else:
    print('Este código se ejecuta por defecto ya que no se cumplio la condición..')
print('fin del código')
```

**Ejemplo IF ELIF y ELSE**

```python
valor_1=int(input('Ingresa un número cualquiera sin coma y sin punto: '))
valor_2=int(input('Ingresa otro número cualquiera sin coma y sin punto: '))
if valor_1==valor_2:
    print('este código se ejecuta porque se cumplio la condición, en este caso que ambos sean iguales..')
elif valor_1>valor_2:
    print("Este código se ejecuta ya que no se cumplio la primer condición pero si está..")
else:
    print('Este código se ejecuta por defecto ya que no se cumplio la condición..')
print('fin del código')
```

Ahora un par de aclaraciones en base a los ejemplos,  
La estructura de if y elif siempre es

```python
if condición:
    tabulación o sangria
```

un elif siempre va despues de un if no puede ir antes y al igual que el if tiene la misma estructura.
en el caso del else como es lo que se ejecuta por defecto no lleva una condición.  
Observen que también ya que en python no existen las llaves para abrir y cerrar se hace la separación por sangria o tabulaciones, fijense como _if_, _elif_ y _else_ estan dentro de la misma columna o nivel, si ponemos el _elif_ con **sangria** es como que si estuviera anidado en el primer _if_.

```python
if condición:
    sangria
elif condición:
    sangria
else:
    sangria
```

## Ejercicio

Vas a generar un código que va a tomar 1 valor de entrada que sera la edad de la persona y vas a comparar con lo siguiente.

Según la edad tendra acceso a 3 secciones o no tendra acceso.

- Si son mayores de 25 años tienen acceso a la zona VIP
- Si son mayores a 18 años pero menores de 25 zona Común
- Si son menores de 18 años pero mayores a 16 años tienen acceso a la matine
- Si son menores de 16 años no pasan.

## Si lo completaste Felicitaciones 🥳
