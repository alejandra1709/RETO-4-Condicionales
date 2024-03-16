# RETO-4-Condicionales
>***1. Dado un número entero, determinar si ese número corresponde al código ASCII de una vocal minúscula.***
```python
num: int = int(input("Escriba un número entero: "))
letra: str = chr(num)
if num==97 or num==101 or num ==105 or num==111 or num==117:
    print ("El número ",num,"( =",letra,") SÍ corresponde al código ASCII de una vocal en minúscula")
else:
    print ("El número ",num,"( =",letra,") NO corresponde al código ASCII de una vocal en minúscula")
```
>***2. Dada una cadena de longitud 1, determine si el código ASCII de primera letra de la cadena es par o no.***
```python
cadena: str = input("Ingrese una letra (cadena de longitud 1): ")
ascii=ord(cadena)
if ascii%2==0:
    print("El código ASCII que le corresponde a la letra" ,cadena, "es un número par (",ascii,")")
else:
    print("El código ASCII que le corresponde a la letra" ,cadena, "es un número impar (",ascii,")")
```
>***3. Dado un carácter, construya un programa en Python para determinar si el carácter es un dígito o no.***
```python
caracter : str = input("Ingrese un caracter: ")
codigo_caracter : int = ord(caracter)
if codigo_caracter>=48 and codigo_caracter<=57:
    print("El caracter ingresado es un dígito (",caracter,")")
else:
    print("El caracter ingresado NO es un dígito (",caracter,")")
```
>***4. Dado un número real x, construya un programa que permita determinar si el número es positivo, negativo o cero. Para cada caso de debe imprimir el texto que se especifica a continuación:***
>
>Positivo: "El número x es positivo"
>
>Negativo: "El número x es negativo"
>
>Cero (0): "El número x es el neutro para la suma"
```python
real : float = float(input("Ingrese un número real: "))
if real>0:
    print("El número",real,"es positivo")
elif real<0:
    print("El número",real,"es negativo")
else:
    print("El número",real,"es el neutro para la suma")
```
>***5. Dado el centro y el radio de un círculo, determinar si un punto de R2 pertenece o no al interior del círculo.***
```python
puntoX_centro : float = float(input("Escriba la abscisa del centro de la circunferencia: "))
puntoY_centro : float = float(input("Escriba la ordenada del centro de la circunferencia: "))
radio : float = float (input("Escriba el radio de la circunferencia: "))
puntoX_R2: float = float(input("Escriba la abscisa del punto a evaluar: "))
puntoY_R2: float = float(input("Escriba la ordenada del punto a evaluar: "))
if (puntoX_R2-puntoX_centro)**2 + (puntoY_R2-puntoY_centro)**2 < radio**2:
    print("El punto (",puntoX_R2,",",puntoY_R2,") pertenece al interior de la circunferencia")
elif (puntoX_R2-puntoX_centro)**2 + (puntoY_R2-puntoY_centro)**2 == radio**2:
    print("El punto (",puntoX_R2,",",puntoY_R2,") es parte de la circunferencia")
else:
    print("El punto (",puntoX_R2,",",puntoY_R2,") no pertenece al interior de la circunferencia")
```
>***6. Dadas tres longitudes positivas, determinar si con esas longitudes se puede construir un triángulo.***
```python
primera_longitud : float = float(input("Escriba la primera longitud en centímetros: "))
segunda_longitud : float = float(input("Escriba la segunda longitud en centímetros: "))
tercera_longitud : float = float(input("Escriba la tercera longitud en centímetros: "))
if primera_longitud+segunda_longitud>tercera_longitud and primera_longitud+tercera_longitud>segunda_longitud and segunda_longitud+tercera_longitud>primera_longitud:
    print("Sí es posible construir un triángulo con las longitudes",primera_longitud,",",segunda_longitud,"y",tercera_longitud)
else:
    print("No es posible construir un triángulo con las longitudes",primera_longitud,",",segunda_longitud,"y",tercera_longitud)
```
