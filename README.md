# Programacion-Funcional
## Tercer Semestre

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

```

```

```

```

```

```

```

```

```

```

```

```

```

```

```








