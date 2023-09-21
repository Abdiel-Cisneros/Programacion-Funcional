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





