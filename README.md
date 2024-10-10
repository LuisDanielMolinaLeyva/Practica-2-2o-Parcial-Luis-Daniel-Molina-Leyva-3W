# Practica-2-2o-Parcial-Luis-Daniel-Molina-Leyva-3W

#Presentacion
print("Bienvenido a la Practica 2 2do Parcial-Luis Daniel Molina Leyva 3W!")
print(" ")

username = input("Introducir nombre de usuario: ")
print("Hola " + username + " !Bienvenido¡")

print(" ")

print("Programa que calcula el factorial")
numero = int(input("Introduzca el número: "))
factorial = 1
i = 1
while (i <= numero):
    factorial = factorial * i
    i = i + 1
print ("El factorial de " + str(numero) + " es " + str(factorial))

print(" ")

# Definir el porcentaje de IVA
porcentaje_iva = 0.21

# Ingresar el precio base del producto
precio_base = float(input("Introduce el precio base del producto: "))

# Calcular el IVA
iva = precio_base * porcentaje_iva

# Calcular el precio final
precio_final = precio_base + iva

# Mostrar los resultados
print(f"Precio base: {precio_base:.2f} $")
print(f"IVA ({porcentaje_iva*100}%): {iva:.2f} $")
print(f"Precio final con IVA: {precio_final:.2f} $")

print(" ")

import math

def area_circulo(radio):
    """Calcula el área de un círculo dado su radio."""
    return math.pi * radio ** 2

def volumen_cilindro(radio, altura):
    """Calcula el volumen de un cilindro dado su radio y altura."""
    area_base = area_circulo(radio)
    return area_base * altura

# Ejemplo de uso
radio = float(input("Introduce el radio: "))  # puedes cambiar este valor
altura = float(input("Introduce la altura: "))  # puedes cambiar este valor

# Calcular el área del círculo
area = area_circulo(radio)
print(f"El área del círculo de radio {radio} es: {area:.2f}")

# Calcular el volumen del cilindro
volumen = volumen_cilindro(radio, altura)
print(f"El volumen del cilindro de radio {radio} y altura {altura} es: {volumen:.2f}")

![image](https://github.com/user-attachments/assets/3603f19c-fe31-4820-aea8-ffd266b72317)
![image](https://github.com/user-attachments/assets/11d1585d-f3aa-4351-93c7-0f9c6a99a475)
![image](https://github.com/user-attachments/assets/67a1e230-a9b5-4631-af8e-99b49a809f42)

#Presentacion
print("Bienvenido a la Practica 2 2do Parcial-Luis Daniel Molina Leyva 3W!")
print(" ")

username = input("Introducir nombre de usuario: ")
print("Hola " + username + " !Bienvenido¡")

print(" ")

def es_email_valido(email):
    """Verifica si el email contiene '@'."""
    return '@' in email

# Capturar la dirección de email del usuario
email_usuario = input("Introduce tu dirección de email: ")

# Verificar si el email es válido
if es_email_valido(email_usuario):
    print("La dirección de email es válida.")
else:
    print("La dirección de email no es válida. Asegúrate de incluir '@'.")

print(" ")

def longitud_ultima_palabra(frase):
    """Devuelve la longitud de la última palabra en un string."""
    # Eliminar espacios en blanco al principio y al final, y dividir en palabras
    palabras = frase.strip().split()
    # Verificar si hay palabras en la lista
    if palabras:
        # Retornar la longitud de la última palabra
        return len(palabras[-1])
    else:
        return 0  # En caso de que no haya palabras

# Ejemplo de uso
frase_usuario = input("Introduce una frase: ")
longitud = longitud_ultima_palabra(frase_usuario)
print(f"La longitud de la última palabra es: {longitud}")

print(" ")

def mayor_de_tres(num1, num2, num3):
    """Devuelve el mayor de tres números."""
    return max(num1, num2, num3)

# Ejemplo de uso
numero1 = float(input("Introduce el primer número: "))
numero2 = float(input("Introduce el segundo número: "))
numero3 = float(input("Introduce el tercer número: "))

mayor = mayor_de_tres(numero1, numero2, numero3)
print(f"El mayor de los tres números es: {mayor}")

print(" ")

![image](https://github.com/user-attachments/assets/1e90662d-9ab7-453d-9040-b1f6f6a135d1)
![image](https://github.com/user-attachments/assets/159e3c08-33cf-4ae0-8694-dc92bd79a25d)
![image](https://github.com/user-attachments/assets/6647f3ed-9dd5-45d6-a685-59e8102d5af9)

#Presentacion
print("Bienvenido a la Practica 2 2do Parcial-Luis Daniel Molina Leyva 3W!")
print(" ")

username = input("Introducir nombre de usuario: ")
print("Hola " + username + " !Bienvenido¡")

print(" ")

def sum(lista):
    """Devuelve la suma de todos los números en la lista."""
    total = 0
    for numero in lista:
        total += numero
    return total

def multip(lista):
    """Devuelve el producto de todos los números en la lista."""
    total = 1
    for numero in lista:
        total *= numero
    return total

# Ejemplo de uso
numeros = [1, 2, 3, 4]

suma_total = sum(numeros)
producto_total = multip(numeros)

print(f"La suma de la lista es: {suma_total}")
print(f"El producto de la lista es: {producto_total}")

print(" ")

def es_vocal(caracter):
    """Devuelve True si el carácter es una vocal, False de lo contrario."""
    vocales = 'aeiouAEIOU'  # Incluyendo mayúsculas y minúsculas
    return caracter in vocales

# Ejemplo de uso
caracter_usuario = input("Introduce un carácter: ")

if len(caracter_usuario) == 1:  # Verifica que se ha ingresado solo un carácter
    resultado = es_vocal(caracter_usuario)
    print(f"¿El carácter '{caracter_usuario}' es una vocal? {resultado}")
else:
    print("Por favor, introduce solo un carácter.")

print(" ")

import math

def distancia_dirigida(punto1, punto2):
    """Calcula la distancia dirigida entre dos puntos en el plano 2D."""
    x1, y1 = punto1
    x2, y2 = punto2
    distancia = math.sqrt((x2 - x1) ** 2 + (y2 - y1) ** 2)
    return distancia

# Ejemplo de uso
punto_a = (float(input("Introduce la coordenada x del primer punto: ")),
            float(input("Introduce la coordenada y del primer punto: ")))

punto_b = (float(input("Introduce la coordenada x del segundo punto: ")),
            float(input("Introduce la coordenada y del segundo punto: ")))

distancia = distancia_dirigida(punto_a, punto_b)
print(f"La distancia dirigida entre los puntos {punto_a} y {punto_b} es: {distancia:.2f}")

print(" ")

![image](https://github.com/user-attachments/assets/9ef0c371-fab1-475f-8ee8-19fe097626ba)
![image](https://github.com/user-attachments/assets/6f72bd4b-909e-46da-9222-294eae38a06a)
![image](https://github.com/user-attachments/assets/7bb75648-8c42-4333-8773-141b0b1e17a3)








