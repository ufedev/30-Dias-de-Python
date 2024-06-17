## [30-Días-de-Python](./../README.md)

# Día 5

## Operaciones aritmeticas

Ningún lenguaje seria util si no se pueden realizar operaciones artimeticas 😆.
En python existen todas y vamos a verlas a continuación.

- vamos a suponer que tenemos 2 números x

```python
numero_1 = 20
numero_2 = 5

# Suma
print(numero_1 + numero_2)

# Resta
print(numero_1 - numero_2)

# Multiplicación
print(numero_1 * numero_2)

# División
print(numero_1 / numero_2)

# Modulo o Resto de división
print(numero_1 % numero_2)
# Si la division de 20/5 deja resto nos mostrara eso.
# En este caso dara 0 porque 5 entra exactamente 4 veces sin que sobre nada.

# División redondeada
print(numero_1 // numero_2)
# Al igual que la división nos da el resultado de la misma pero redondea si hay decimales al valor mas proximo.

# Potencia
print(numero_1 ** numero_2) # Fijese que hay 2 asteriscos(*) seguidos




```

### Para el ejercicio que queremos que sea mas interactivo vamos a aprender algo sobre los tipos de datos.

La función _input_ siempre devuelve un texto **str** nosotros para realizar las operaciones aritmeticas
necesitamos que sean números **int** o **float**, para esto python nos ofrece funciones que transforman el tipo de dato:

- int() -> transfroma a entero
- float() -> transforma a decimal
- str() -> transforma a texto

Existen mas pero estas son las que nos interesan por el momento.

_Como aplicarlas_

```python

mi_numero="1" #Fijese que esta entre comillas lo que significa que para python es un texto no un número

print(int(mi_numero))
# 1

print(float(mi_numero))
# 1.0

print(str(mi_numero))
# 1


```

En el ultimo caso no realizara ningún cambio ya que la variables esta como texto _str_.
En los 2 primeros ejemplos cuando se imprima por pantalla el color cambiara ya que es otro tipo de dato.

Podemos ver el tipo de dato que es con la función predefinida en python llamada **type()**

```python


mi_numero="1" #Fijese que esta entre comillas lo que significa que para python es un texto no un número

print(type(mi_numero))
#<class 'str'>

print(type(int(mi_numero)))
#<class 'int'>

print(type(float(mi_numero)))
#<class 'float'>

```

### Ejercicio:

- Pide al usuario que ingrese 2 números mayores a 0(cero) y enteros y realiza las siguientes operaciones y muestre en pantalla:
  - Suma
  - División
  - Potencia

_Recuerda que los **input** siempre devuelven texto **str** por lo tanto deberas transformarlos en un número para poder realizar las operaciones aritmenticas sin errores_

### Felicitaciones 🎊
