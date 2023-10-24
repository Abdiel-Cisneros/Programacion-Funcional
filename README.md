# Programacion-Funcional
## Tercer Semestre
## Notas de clase


En este semestre se dedicará al Lenguaje de Programación Python


## Primera Parcial

### ----22/08/2023----
Calculadora

___¿Qué es la programación funcional?___

Paradigma de programacion que considera el computo como la evaluacion de funciones
matemáticas que evitan los cambios de estado y los datos mutables.

```
while True:
    print("\nMi Calculadora")
    print("1. Suma")
    print("2. Resta")
    print("3. Multiplicación")
    print("4. División")
    print("5. Salir")

    opcion = input("Selecciona una opción: ")

    if opcion == '5':
        print("¡Hasta luego!")
        break

    num1 = float(input("Ingresa el primer número: "))
    num2 = float(input("Ingresa el segundo número: "))

    if opcion == '1':
        print("Resultado:", num1 + num2)
    elif opcion == '2':
        print("Resultado:", num1 - num2)
    elif opcion == '3':
        print("Resultado:", num1 * num2)
    elif opcion == '4':        
        if num2 != 0:
            print("Resultado: ", num1 / num2)
        else:
            print("No se puede dividir entre cero")
    else:
        print("¡Gracias por usar Mi Calculadora!")
```

### ----25/08/2023----

```
numero:int = 10
numero = "dos"
print(numero)

#Análisis estático de código

""" 
--Version 1--

num= 0;
n = int(input("Dame un número entero positivo"))
if n%2 == 0:
    num = "Par"
else:
    num = "Impar"
 """


#?--Version 2--
""" 
n = int(input("Dame un numero entero positivo"))
(num:="par" if n%2 == 0 else "impar")
 """

# casting
# Conversión de tipos
num_str = "3"
num_int = int(num_str)
print(f"num_int: (num_int)") #fstrings

num_float = 3.14
num_int = int(num_float)
num_int(f"num_int: (num:int)")

num_str = str(num_float)
print(f"num_str: (num_str)")
num_str

def res():
    num_str = "3"
    num_str = "10"
    return (num_str, num_int)

num_str = str(num_float)
res_tupla = (num_str, num_int)
print(f"num_st" (variable) a: Literal['3'])
print(f"res: %")

a, b = res() #unzip
print(f"res: {a} {b}")
```

Durante varias clases, hemos utilizado Jupyter

### ----29/08/2023----

```
nombre: str = "Hugo"
print(nombre)
print(type(nombre))
nombre.capitalize()
# Capitalizar hace que la primera letra sea en Mayúsculas
nombre.upper()
```

```
numero: int = 10
pi:float = 3.14
es_alumno: bool = True
name:syt= "Hugo"

print(f"{num}-{pi}-{name}")
# f Strings
```

```
print(5+4)
print(5-4)
print(5*4)
print(5/4)
print(5//4) #División entera 
print(5%4) # Módulo o residuo 
print(5**4) # x a la y
```

```
print(True and False)
print(True or False)
print(not False)
```
CONDICIONALES

```
n1: int = 10
n2: int = 20

if n1 > n2:
    print(f"{n1}>{n2}")
```

```
n1: int = 10
if n1 > n2:
    print(f"{n1}>{n2}")
else:
    print(f"{n1}<{n2}")
```


```
edad: int = 18

if edad >= 18:
    print("mayor de edad")
    elif edad == 18:
        print("Acabas de llegar a la mayoría de edad")
    else:
        print("eres menor de edad")
```

```
match True:
    case "edad == 18":
        print("Acabas de llegar a la mayoría de edad")
    case edad > 18:
        print("Eres mayor de edad")
    case edad <s 18:
        print("Eres menor de edad")
```

### ----05-09-2023----

```
# Listas 
# Collections
def suma(a + b):
    return a + b 
def resta(a - b):
    return
def multiplicacion(a * b):
    return
def division(a / b):
    return a / b
operaciones = [suma,resta, multiplicacion, division]

```


```
#Lista

def suma(a,b):
    pass

print(suma(3,4))
#Retorna None
```


```
def operaciones (a,b):
    return a+b, a-b, a*b, a/b

respuestas = operaciones(5,4)
print(respuestas)
w,x,y,z = operaciones(5,4)
print(w)
```


```
res_suma._._._ = operaciones(5,4)
res_suma
```


```
#Tuple
#La tupla es inmutable
tupla_funciones = (suma,resta,multiplicacion,division)
print(tupla_funciones[0](5,4))

tupla = [1,2,4,5,True,4,5,"Hola",[1,2,3]]
```


```
#tupla[0]=10 #Es inmutable
lista.append(10)
lista

tupla.__add__((10,10))


def suma(a: int,b :int) -> int:
    return a + b

def operacion (a:int , b:int) -> [int, int]:
    return (a+b, a-b)

(a,b) = operacion(5,6)
a,b = operacion(0,5)
print(a,b)
```


```
#range
#Permite crear un iterable desde 0 hasta -1
numeros = range(10)
print(numeros)

range(0,10)
```


```
for i in numeros:
    print(i, end= " ")
```


```
numeros = range(5,10)
numeros
```


```
for i in numeros:
    print(i,end=" ")
```


```
numeros_pares = range(2,11,2)
for par in pares:
    print(par,end=" ")
```


```
for item in range(2,11,2):
    print(item, end=" ")
```


```
list(numeros)
```


```
numeros = list(numeros)
```


```
lista = [3,6,7,48,34, 67, 89]
max(lista)
```


```
lista = [3,6,7,48,34, 67, 89]
min(lista)
```


```
sum(lista)
```


```
sorted(lista)
```


```
lista = [3,6,7,48,34, 67, 89]
```


```
lista.sort()
```


```
print(lista.sort())
```

```
lista.sort(reverse-True)
lista
```


```
# Set conjuntos

mi_set = [1,2,3,3,3,3]
mi_set
```


```
data= [15,14,13,1,2,3,4,5,6,7,8,9,1,2,1,2,1]

list(set(data))
```


```
data2 = [1,56,57,58]

mi_set.union(data2)

```


```
#Diccionarios

mi_dictionary = [ "Llave": "valor" ]
mi_dictionary["llave"]
```



```
mi_dictionary.keys()
```


```
mi_dictionary.values(['valor'])
```


```
for e in mi_set:
    print(e)

for key in days_of_the_week.keys():
    print(key,end=" ")

```

### ----08/09/2023----

En una carpeta llamada Milibreria se encuentran 2 archivos

#### resta.py
```
def resta (a:int, b:int) ->int:
    return a - b
```

#### suma.py

```
def suma(a: int ,b: int) ->int:
    return a + b


def suma2(a:float, b:float)-> float:
    return a + b


def suma1(a: int|float, b: int|float)-> int|float:
# La línea indica que la variable puede 
    return a + b
if __name__ == "__main__":
    print(suma(5,6))
```


### 12/09/2023

Dentro de la carpeta llamda Webpage se encuentran estos archivos

-Durante la clase, nos enseñaron la libreria _Streamlit_


#### agendamain.py

```
from dataclasses import dataclass

@dataclass #decorators

#Definiendo la clase
class User:
    
 id: str
 name: str
 age: int

 def show_data():
     return f"10: (id)\nNombre: (self.name)\nEdad: (self.age)"

 #instancia
if __name__ == "__main__":
    usuario1 = User("1","Hugo",25)
    usuario2 = User("1","Paco",25)
    usuario3 = User("1","Luis",25)
    usuario4 = User("1","Vladi",25)
    usuarios = [usuario1, usuario2, usuario3, usuario4]
    for usuario in usuarios:
       print(usuario.show_data())

```

#### main.py

```
import streamlit as st

# st.write("Hola ICI")

st.sidebar.title("Calculadora ICI")

def pedir_valores():
    name = st.text_input("Nombre:")
    n1 = st.number_input("Número 1:")
    n2 = st.number_input("Número 2:")

    if st.button("Sumar"):
        st.succes("sumando...")
        st.write(f"{n1} + {n2} = {n1 + n2}")

opcion = st.sidebar.selectbox("Opciones:",[
    "Suma", "Resta", "Multiplicación", "División", "A cerca de"
    ])

match opcion:
    case "Suma":
        st.write("Esta es la opcion de suma...")
    case "Resta":
        st.write("Esta es la opcion de Resta...")
    case "Multiplicación":
        st.write("Esta es la opcion de Multiplicación...")
    case "División":
        st.write("Esta es la opcion de División...")
    case "A cerca de":
        st.write("Derechos Reservados")
        st.write("UCOL FIME ICI ")
```

#### operacionesmain.py

```
import milibreria.suma as lib
import milibreria.resta as lib 

from milibreria import suma,resta
import milibreria as lib




if __name__ == "__main__":
    print(suma.suma(7,8))
    print(resta.resta(8,4))

# el main es el enter point del programa
```

#------------------------------------------------------------------------------------------------------------------------------------------------------------
## Segunda Parcial

#-Notas de Jupiter 
```
def my_function(my_list=[]): #La lista no tiene argumentos
    my_list.append('???')
    return my_list
```

```
my_function(["a","b","c"])
```

```
global num
num = 10
#Python permite definir por fuera de las funciones, pero no significa que
#sea una buena práctica, se debe de evitar

def a():
    print(num)
    num=10

def b():
    y= num+10
    print(y)

a()
b()

num=10
print(id(num))

def c():
    x= x+1
    print(x)
c()
print(x)
print(id(x))
```

```
def double(x):
    x*=2
    print(x)
    #return x

x = 5
x= double(x)
x
print(x)
```

```
def double_lista(x):
    i=0
    while i < len(x):
        x[1] *=2
        i+=1
    print(x)
   
a=[1,2,3,4,5]
a= double_lista(a)
a
```

```
names = dict(name_1="Hugo",name_2="Paco",name_3="Luis")
names
```

```
def f():
    return dict(name_1="Hugo",name_2="Paco",name_3="Luis")


f()
```

```
f()['Name_3']
```

```
#Argumentos nombrados, argumentos posicionales obligatorios
```

```
print("Hola")


#! Argumentos de palabra Clave

'''
A partir del asterisco, todos los demás son nombrados o de llaves



-Argumentos de llave o asterisco
'''

#? Diccionarios

```

### Clase del día 17 / 10 / 2023
#### Se creó una carpeta llamada "Calculadora"
#### -Dentro de la carpeta hay un archivo llamado "__init__.py", la cual no contiene nada
#### -Dentro de la carpeta está otro archivo llamado "Calculos.py" el cual contiene lo siguiente:

```
def suma(a,b):
    """
    Comentarios de la función suma
    """
    return a + b

def resta(a,b):
    return a - b

def multiplicacion(a,b):
    return a * b

def division(a,b):
    if b ==0:
        raise ZeroDivisionError("division by zero")
    return float(a/b)

def cuadrado(a):
    return a ** 2

```

#### Fuera de la carpeta de "Calculadora" se encuentra un archivo llamado "main_calculadora.py" la cual se utilizará para demostrar las distintas maneras de poder importar los archivos usando distintos modos, siendo uno de ellos es el alías para llamar de una manera en específica una función dentro del archivo, el * que nos sirve para importar todas las funciones, también se puede solamente importando la función del archivo que necesitamos para nuestro programa.

```
#import Calculadora.calculos as calc #alias

#print(calc.suma.__doc__)
#print(calc.suma(2,3))

#------------------------------------------------------------------

#from Calculadora import calculos

#print(calculos.suma(2,3))
#print(calculos.resta(2,3))
#print(calculos.multiplicacion(2,3))
#print(calculos.division(2,3))
#print(calculos.cuadrado(2))

#------------------------------------------------------------------

#from Calculadora.calculos import *

#print(suma(2,3))
#print(resta(2,3))

#------------------------------------------------------------------

#from Calculadora.calculos import suma

#print(suma(2,3))
#print(resta(2,3))

#------------------------------------------------------------------

#from Calculadora.calculos import suma as sumar #Alias o sobrenombre  #Aka
#from Calculadora.calculos import suma as restar

#print(sumar(2,3))
#print(restar(2,3))

#------------------------------------------------------------------

from Calculadora.calculos import suma as sumar, resta as restar

#alias aka=as know as

print(sumar(2,3))
print(restar(2,3))
```

## -----Notas Jupiter de Classroom------

### 2.1.4 Funciones como Objetos
#### 2.1.4.1 Asignación de funciones a variables.
##### Escriba una función double que obtenga el doble de un valor mediante el uso de una variable.

```
# Definir la función double
def double(x:int)->int:
    return x * 2

# Asignar la función double a la variable my_double
my_double = double
print(type(my_double))

# Llamar a la función a través de la variable
result = my_double(5)

# Imprimir el resultado
print(result)
```

* Este programa define una función llamada `double` que toma un argumento `x` y devuelve el doble del mismo.
* La función `double` se asigna a la variable `my_double`.
* La función `my_double` se llama con el argumento 5 y el resultado se asigna a la variable `result`. 
* Finalmente, el programa imprime el valor de `result` en la pantalla, que es el resultado de llamar a la función `double` con el argumento 5.

#### 2.1.4.2 Paso de funciones como argumentos.

##### Escriba un programa que mediante el uso de dos funciones: double() y cuad(), se pueda obtener el cuadrado del doble de un número entero. La función double debe ser usada como argumento de cuad.

```
def double(x:int)->int:
    return x * 2

# Llamar a la función a través de la variable
doble = double(3)

def cuad(f):
    return f ** 2

cuadrado = cuad(doble)
print(cuadrado)

```

* Este programa define dos funciones, `double` y `cuad`
* las utiliza para calcular el cuadrado del doble de un número. 
* Primero, la función `double` multiplica su argumento por 2 y lo devuelve.
* Luego, la función `cuad` toma un argumento `f` y devuelve el cuadrado de `f`.
* El programa asigna la función `double` a la variable `my_double`, llama a `my_double` con el argumento 5 y asigna el resultado a la variable `doble`.
* Finalmente, el programa llama a `cuad` con `doble` como argumento y asigna el resultado a la variable `cuadrado`, que se imprime en pantalla.

##### Escriba ahora un programa que eleve una lista de números al cuadrado. La función se debe llamar elevar_numeros y debe recibir como argumento la lista y la función cuad, que es la que va a elevar el número al cuadrado.

```
def cuad(n:int)->int:
    return n ** 2


def elevar_numeros(lista, cuad):
    lista_cuadrados = []
    for num in lista:
        lista_cuadrados.append(cuad(num))
    return lista_cuadrados


lista = [1, 2, 3, 4, 5]
print(elevar_numeros(lista, cuad))
```



```
def cuad(n:int)->int:
    return n ** 2


def elevar_numeros(lista):
    lista_cuadrados = []
    for num in lista:
        lista_cuadrados.append(cuad(num))
    return lista_cuadrados


lista = [1, 2, 3, 4, 5]
print(elevar_numeros(lista))

```



```
def elevar_numeros(lista):
    lista_cuadrados = []
    for num in lista:
        lista_cuadrados.append((lambda x: x **2)(num))
    return lista_cuadrados


lista = [1, 2, 3, 4, 5]
print(elevar_numeros(lista))

```

* Este programa define dos funciones, `cuad` y `elevar_numeros`, se utilizan para calcular el cuadrado de cada número en una lista.
* La función `cuad` toma un argumento `n` y devuelve el cuadrado de `n`.
* La función `elevar_numeros` toma una lista y una función como argumentos, y devuelve una lista que contiene el resultado de aplicar la función a cada elemento de la lista original.
* En este caso, la función `elevar_numeros` llama a la función `cuad` para cada número en la lista y devuelve una lista de los cuadrados correspondientes.
* El programa crea una lista de números del 1 al 5, llama a la función `elevar_numeros` con la lista y la función `cuad` como argumentos, y luego imprime la lista resultante de cuadrados en la pantalla.

##### Escriba un programa que eleve a la potencia y cada uno de los elementos de una lista. Use la función elevar_números que reciba la lista y la potencia, y dentro de esta use la función potencia que se encargará de elevar a la potencia y cada elemento de la lista.

```
def potencia(x,y): #pow(x,y)
    for _ in range(y):
        x = x * y
    return x


def elevar_numeros(lista, y):
    lista_potencias = []
    for num in lista:
        lista_potencias.append(pow(num,y))
    return lista_potencias


lista = [1, 2, 3, 4, 5]
print(elevar_numeros(lista, 2))

```

* Este programa define dos funciones: `potencia` y `elevar_numeros`
* Permite elevar cada número en una lista a una potencia dada.
* La función `potencia` toma dos argumentos, `x` y `y`, y devuelve `x` elevado a la potencia `y`.
* La función utiliza un ciclo `for` para multiplicar `x` por `y` `y` veces.
* La función `elevar_numeros` toma una lista y un número `y` como argumentos, y devuelve una lista que contiene el resultado de elevar cada elemento de la lista a la potencia `y`.
* La función `elevar_numeros` llama a la función `potencia` para cada número en la lista y agrega el resultado a una nueva lista.
* El programa crea una lista de números del 1 al 5, llama a la función `elevar_numeros` con la lista y el número 2 como argumentos, y luego imprime la lista resultante de números elevados al cuadrado en la pantalla.



#### 2.1.4.3 Funciones anónimas (lambda functions).

Las funciones lambda en Python son funciones anónimas que se pueden definir en una sola línea de código. 

- Las funciones lambda:
    * se definen utilizando la palabra clave `lambda`, seguida de los argumentos de la función separados por comas y luego dos puntos.
    * es una expresión que se evalúa y devuelve como resultado.
    - son funciones anónimas, lo que significa que no tienen un nombre definido.
    - se pueden asignar a una variable y luego llamar a través de esa variable.
    - se utilizan comúnmente como argumentos de otras funciones, como `map()`, `filter()`, `reduce()`, etc.
    - son útiles para escribir código más conciso y legible (cuando se trabaja con funciones simples y de una sola línea)

```
def identity(x):
    return x

print(identity(3))
```

```
lambda x: x
#print((lambda x: x*2)(5))
y = lambda x: x
y(5)
```

```
cuadrado = lambda x: x+1
cuadrado(3)
```

```
lambda x: x + 1
```

```
(lambda x: x + 1)(2)
```

```
# puede ser nombrada
add_one = lambda x: x + 1
add_one(2)
```

```
def add_one(x):
    return x + 1
```

```
(lambda x,y: x/y)(10,y=1)

def division(x,y=1):
    return x/y
 
 
division(5)   
```

### 2.1.5 Recursión

#### 2.1.5.1 Definición de funciones recursivas.

* Una definición recursiva es aquella en la que el término definido aparece en la propia definición.
* Capacidad de una función de llamarse a sí misma
* La mayoría de los problemas de programación se pueden resolver sin recursividad. 
* Entonces... la recursividad no suele ser necesaria.
--------
* El recorrido de estructuras de datos en forma de árbol es un ejemplo.
* Debido a que se trata de estructuras anidadas, se ajustan fácilmente a una definición recursiva.
* Es probable que un algoritmo no recursivo para recorrer una estructura anidada sea algo burdo.
* Una solución recursiva puede ser más elegante y eficiente.

```
def f():
    x = 10
    f()
```

```
f()
```

```
# Para conocer el límite de recursión
import sys
print(sys.getrecursionlimit())
```

```
from sys import getrecursionlimit
print(getrecursionlimit())
```

```
# Se puede modificar el límite de recursión
sys.setrecursionlimit(500)
```

```
f()
```

* Las funciones recursivas suelen un patrón:
    * Hay uno o más casos base que se pueden resolver directamente sin necesidad de más recursividad.
    * Cada llamada recursiva acerca progresivamente la solución a un caso base (mecanismo de retorno).


#### 2.1.5.2 Casos base y casos recursivos.

* Ejemplo: Cuenta regresiva hasta cero

```
# cuenta regresiva no recursiva (iterativa)
def cuenta_regresiva(n):
    while n >= 0:
        print(n)
        n -= 1

cuenta_regresiva(5)
```

```
# cuenta regresiva recursiva
def cuenta_regresiva(n):
    print(n)
    if n == 0:
        return                      # Fin de la recursión, caso base
    else:
        cuenta_regresiva(n - 1)     # Llamada recursiva


cuenta_regresiva(5)
```

* El caso base se produce cuando n es cero, momento en el que se detiene la recursividad.
* En la llamada recursiva, el argumento es uno menos que el valor actual de n, por lo que cada recursividad se acerca al caso base.

* Ejemplo: Calcular el factorial

```
# Función factorial no recursiva (iterativa)
def factorial(n):
    result = 1
    for i in range(1, n+1):
        result *= i
    return result
```

```
# función factorial recursiva
def factorial(n):
    if n == 0:
        return 1
    else:
        return n * factorial(n - 1)

print(factorial(5))
```

```
def factorial(n):
    return 1 if n <= 1 else n * factorial(n - 1)


print(factorial(5))
```

```
def factorial(n):
    print(f"factorial() llamado con n = {n}")
    return_value = 1 if n <= 1 else n * factorial(n -1)
    print(f"-> factorial({n}) retorna {return_value}")
    return return_value


factorial(5)
```

* Calcular el tiempo de ejecución (evaluación empírica)
* timeit(<command>, setup=<setup_string>, number=<iterations>)

```
# Ejemplo iterativo
from timeit import timeit

timeit("print(string)", setup="string='Hola Mundo'", number=100)
```


```
# Performance algoritmo factorial iterativo
from timeit import timeit

setup_string = """
print("Iterativo:")
def factorial(n):
    result = 1
    for i in range(2, n + 1):
        result *= i
    return result
"""

from timeit import timeit
timeit("factorial(4)", setup=setup_string, number=10000000)
```

```
# Performance algoritmo factorial iterativo recursivo
from timeit import timeit

setup_string = """
print("Recursive:")
def factorial(n):
    return 1 if n <= 1 else n * factorial(n - 1)
"""

from timeit import timeit
timeit("factorial(4)", setup=setup_string, number=10_000_000)
```

```
#Usando reduce
setup_string = """
from functools import reduce
print("reduce():")
def factorial(n):
    return reduce(lambda x, y: x * y, range(1, n + 1) or [1])
"""

from timeit import timeit
timeit("factorial(5)", setup=setup_string, number=10000000)
```

```
# Python ya tiene una función factorial
from math import factorial
factorial(4)
```

```
setup_string = "from math import factorial"

from timeit import timeit
timeit("factorial(4)", setup=setup_string, number=10_000_000)
```

###-----------------------------------------------------------------------------------
### 2.1.6 Documentación y Comentarios
#### 2.1.6.1 Uso de docstrings para documentar funciones.

```
def suma(a, b):
    """
    This function adds two numbers.

    Parameters:
    a (int): The first number.
    b (int): The second number.

    Returns:
    int: The sum of a and b.
    """
    return a + b

def resta(a, b):
    """
    This function subtracts two numbers.

    Parameters:
    a (int): The first number.
    b (int): The second number.

    Returns:
    int: The difference between a and b.
    """
    return a - b

def multiplicacion(a, b):
    """
    This function multiplies two numbers.

    Parameters:
    a (int): The first number.
    b (int): The second number.

    Returns:
    int: The product of a and b.
    """
    return a * b

def division(a, b):
    """
    This function divides two numbers.

    Parameters:
    a (int): The first number.
    b (int): The second number.

    Returns:
    float: The quotient of a and b.
    """
    return a / b

```

```
print(suma.__doc__)
```

#### 2.1.6.2 Comentarios relevantes en el código.

```
def suma(a, b):
    """
    This function adds two numbers.

    Parameters:
    a (int): The first number.
    b (int): The second number.

    Returns:
    int: The sum of a and b.
    """
    # Check if both a and b are integers
    if not isinstance(a, int) or not isinstance(b, int):
        print("Both a and b should be integers.")
        return None
    
    # Add a and b
    result = a + b
    
    # Print the result
    print(f"The sum of {a} and {b} is {result}.")
    
    return result

```

```
print(suma(1.0,5))
```

### 2.1.7 Módulos y Organización:**

#### 2.1.7.1 Creación de módulos con funciones.
1. Crear la carpeta calculadora
2. Crear el archivo __init__.py
3. Crear el archivo que tendrá las funciones: calculos.py
4. Crear las funciones dentro de calculos.py

#### 2.1.7.2 Importación de funciones desde módulos.

### 2.1.8 Pruebas y Depuración:

```

#import unittest


def suma(a, b):
    """
    This function adds two numbers.

    Parameters:
    a (int): The first number.
    b (int): The second number.

    Returns:
    int: The sum of a and b.
    """
    return a + b

def resta(a, b):
    """
    This function subtracts two numbers.

    Parameters:
    a (int): The first number.
    b (int): The second number.

    Returns:
    int: The difference between a and b.
    """
    return a - b

assert suma(2, 3) == 5.0, "debería ser 5"
assert suma(-2, 3) == 1, "debería ser 1"
assert suma(0, 0) == 0, "debería ser 0"
assert suma(-3,-3) == -6, "debería ser -6"
    
assert resta(2, 3) == -1, "debería ser -1"
assert resta(-2, 3) == -5, "debería ser -5"
assert resta(0, 0) == 0, "debería ser 0"
        
```











