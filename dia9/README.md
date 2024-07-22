## [30-Días-de-Python](./..)

# Día 9

## break y continue

Hay 2 palabras clave que no vimos que son 'break' y 'continue' y estas estan ligadas al uso en un bucle.  
Como dicen las palabras cuando las traducimos uno es 'romper' y el otro es 'continuar' respectivamente.

#### Veamos un ejemplo 'break'

```python

"""
Usando bucle for
"""
for numero in range(1,10):
    print(numero)
    if numero == 2:
        break

"""
Usando bucle while
"""

numero = 1

while numero < 10:
    print(numero)
    if numero == 2:
        break


```

> [!NOTE]
> Como vemos estos 2 bucles hacen el mismo recorrido del 1 al 10 sin incluir el 10. dentro de ambos tenemos la misma condicional que si el número es 2 se ejecutara un break, al ejecutarse un break lo que sucedera es que los bucles iran del 1 al 2 terminando su ejecución ahi ya que el bucle 'se rompe'

> [!TIP]
> Copia y proba el código para verlo mejor.

#### Veamos un ejemplo 'continue'

```python

for numero in range(1,10):
    print(numero)
    multiplicacion = numero * 2
    if multiplicacion < 10:
        continue

    print(multiplicacion)

```

> [!NOTE]
> Aquí hay un ejemplo de continue, expliquemos el código. El bucle recorre de 1 a 10 sin incluir el 10. Despues imprime el número, a continuación lo multiplica y guarda en 'multiplicación', si multiplicación es menor a 10 el bucle ejecuta 'continue' y por ultimo fuera del if imprime la multiplicación.

> [!NOTE]
> 'continue' reinicia el bucle desde ahi, digamos siempre que se ejecute continue el bucle vuelve al principio sin ejecutar el código que sigue despues del 'continue'

> [!TIP]
> Copia el código para ver como funciona realmente.

> [!WARNING]
> Proba hacerlo con el bucle while

## Esto es todo por el día 9. Hagamos un mini ejercicio para familiarizarnos más

#### Ejercicio

En un rango del 1 al 20 imprimir todos los números pares, si es impar que la ejecución continue y no se imprima nada.

> [!TIP]
> Recorda la clase del día 5, los modulos o restos. Si el resto de la operación 'número % 2' es igual a 0 significa que es un número par.

## Felicidades por llegar hasta aquí
