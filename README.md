# Reto número 4

Este repositorio contiene la solución a 8 puntos del reto numero 4 de programcion de computadores. 

### Primer Punto - Vocales ASCII

```python
a : int
a = int(input("Ingrese un numero entero: "))
if a == 97:
  print("el numero ingresado corresponde a la vocal minuscula 'a' dentro del codigo ASCII")
elif a == 101:
  print("el numero ingresado corresponde a la vocal minuscula 'e' dentro del codigo ASCII")
elif a == 105:
  print("el numero ingresado corresponde a la vocal minuscula 'i' dentro del codigo ASCII")
elif a == 111:
  print("el numero ingresado corresponde a la vocal minuscula 'o' dentro del codigo ASCII")
elif a == 117:
  print("el numero ingresado corresponde a la vocal minuscula 'u' dentro del codigo ASCII")
else:
  print("el numero ingresado no corresponde a ninguna vocal minuscula en codigo ASCII")
```
Nota: Este codigo evalua numeros enteros que estan relacionados con un valor en ASCII, pero funciona solo para determinar si el numero ingresado pertenece a una vocal en ASCII.

### Segundo Punto - Par o impar ASCII?

```python
a : str
a = (input("ingrese un caracter (solo uno porfavor !!!!!) dentro del alfabeto ingles: "))
sbl_ASCII = ord(a)

if sbl_ASCII % 2 == 0:
  print("el caracter ingresado corresponde a un numero par dentro del codigo ASCII")
else:
  print("el caracter ingresado corresponde a un numero impar dentro del codigo ASCII")
```
Nota: En el segundo punto se pide al usuario que ingrese un caracter del alfabeto ingles cuyo simbolo va a ser traducido a su valor en lenguaje ASCII y luego dividio entre 2 para saber si este valor es par o impar 

### Tercer punto - Digito ASCII?

```python
a: str
a = input("Ingrese un caracter (solo uno por favor) dentro del alfabeto inglés: ")
sbl_ASCII = ord(a)

if sbl_ASCII >= 48 and sbl_ASCII <= 57:
    print("El caracter ingresado corresponde a un dígito dentro del código ASCII")
else:
    print("El caracter ingresado no es un dígito dentro del código ASCII")
```
Nota: En el tercer punto se va a ejecutar un codigo que le pide a un usuario ingresar un caracter y el programa te va a decir si corresponde a un numero dentro del codigo ASCII

### Cuarto punto - Multiplo?

```python
a = float(input("ingrese un numero: "))
b = float(input("ingrese otro numero: "))

print(" ")
if a % b == 0:
  print("El primer numero es multiplo del segundo")
else:
  print("El pirmer numero no es multiplo del segundo")
```
Nota: En el cuarto punto comparamos 2 numeros ingresados y se evaluasi si el primero es multiplo del segundo

### Quinto punto - positivo, negativo o cero?

```python
a = float(input("ingrese un numero x:"))
if a > 0:
  print("El numero x es positivo")
elif a < 0:
  print("El numero x es negativo")
else:
  print("El número x es el neutro para la suma")
```
Nota: En el quinto punto se evalua si un numero ingresado es positivo, negativo o cero

### Sexto punto - Pertene a una circunferencia en un plano?

```python
import random
x = float(input("Ingrese un numero real para la cordenada en x del centro del circulo: "))
y = float(input("Ingrese un numero real para la cordenada en y del centro del circulo: "))

radio = float(input("Ingrese un valor para el radio del circulo 'r': "))

print(" ")
print("Centro del circulo (x,y) = "+"("+str(x)+" , "+str(y)+")"+" y radio: "+str(radio))
print(" ")

x_rand = float(input("Ingrese un numero real para la cordenada en x que desee evaluar en el plano: "))
y_rand = float(input("Ingrese un numero real para la cordenada en y que desee evaluar en el plano: "))

print("Punto aleatorio (x2,y2) ingresado = "+"("+str(x_rand)+" , "+str(y_rand)+")")

print(" ")
if ((x_rand-x)**2 + (y_rand-y)**2) <= radio**2:
  print("El punto R2 esta dentro del circulo")
else:
  print("La coordenada R2 no esta dentro del circulo")
```
Nota: En el sexto punto se le pide al usuario que "cree" un circulo en una plano bidimensional, ingresando una coordenada (x,y) que va a ser el centro de la circunferencia en el pano, y un radio especifico. Esto con el fin que un usuario pueda evaluar si hay un punto que pertenesca a la circunferencia.

### Septimo punto - Multiplo?

```python
L1 = float(input("Ingrese una longitud para el lado 1 del triangulo: "))
L2 = float(input("Ingrese una longitud para el lado 2 del triangulo: "))
L3 = float(input("Ingrese una longitud para el lado 3 del triangulo: "))

print(" ")
print("Medidas lados del triangulo: "+"("+str(L1)+" , "+str(L2)+" , "+str(L3)+")")
print(" ")

if (L1 + L2 > L3) or (L2 + L3 > L1) or (L1 + L3 > L2):
  print("Es posible crear un triangulo con las dimensiones dadas")
else:
  print("No es posible crear un triangulo con las dimensiones dadas")
```
Nota: En el septimo punto se pide que ingresen 3 longitudes para armar un triangulo, y el programa evalua si es posible realizarlo con esas dimensiones.

### Octavo punto - Multiplo?

```python

print("Escriba el nombre de un pais del Continente americano en letras minusculas, sin tildes ni caracteres chimbos, para que le funcione el programa")
pais = str(input("Ingrese el nombre del pais: "))

match pais:
    case "canada":
        print("Capital: Ottawa")
    case "estados unidos":
        print("Capital: Washington D.C.")
    case "mexico":
        print("Capital: Ciudad de México")
    case "belice":
        print("Capital: Belmopan")
    case "costa rica":
        print("Capital: San Jose")
    case "el salvador":
        print("Capital: San Salvador")
    case "guatemala":
        print("Capital: Ciudad de Guatemala")
    case "honduras":
        print("Capital: Tegucigalpa")
    case "nicaragua":
        print("Capital: Managua")
    case "panama":
        print("Capital: Ciudad de Panama")
    case "antigua y barbuda":
        print("Capital: Saint John’s")
    case "bahamas":
        print("Capital: Nasau")
    case "barbados":
        print("Capital: Bridgetown")
    case "cuba":
        print("Capital: La Habana")
    case "dominica":
        print("Capital: Roseau")
    case "granada":
        print("Capital: Saint George’s")
    case "haiti":
        print("Capital: Puerto Príncipe")
    case "jamaica":
        print("Capital: Kingston")
    case "republica dominicana":
        print("Capital: Santo Domingo")
    case "san cristobal y nieves":
        print("Capital: Basseterre")
    case "santa lucia":
        print("Capital: Castries")
    case "san vicente y las granadinas":
        print("Capital: Kingstown")
    case "trinidad y tobago":
        print("Capital: Puerto Espana")
    case "argentina":
        print("Capital: Buenos Aires")
    case "bolivia":
        print("Capital: Sucre (constitucional) y La Paz (sede de gobierno)")
    case "brasil":
        print("Capital: Brasilia")
    case "chile":
        print("Capital: Santiago")
    case "colombia":
        print("Capital: Bogota")
    case "ecuador":
        print("Capital: Quito")
    case "guyana":
        print("Capital: Georgetown")
    case "paraguay":
        print("Capital: Asuncion")
    case "perú":
        print("Capital: Lima")
    case "surinam":
        print("Capital: Paramaribo")
    case "uruguay":
        print("Capital: Montevideo")
    case "venezuela":
        print("Capital: Caracas")
    case _:
        print("País no identificado, asegurese de escribir el nombre del pais segun las condiciones iniciales, porfavor, que me da pereza arreglar sus errores, vea que son las 12 de la noche")
```
Nota: En el octavo punto se pide que un usuario escriba el nombre en minúsculas de un pais de America y retorne la ciudad capital, si el pais no pertenece al continente debe arrojar país no identificado, este codigo se realizo usando 'match-case'.



