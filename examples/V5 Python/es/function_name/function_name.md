category: functions  
signature: def function_name(parameters):\n\tpass  
description: Functions are blocks of code used to perform an action.

# Función

Las funciones son bloques de código que se utilizan para realizar una acción.

## Cómo Utilizar

Para crear una función, cree un nombre de función significativo. Esto significa que el nombre de la función debe describir con precisión lo que hace.

Utilice la **palabra clave** `def` antes del nombre de la función para definir la función.

Incluya paréntesis `()` y encierra parámetros opcionales después del nombre de la función, seguido por un colon`:`. Múltiples parámetros deben estar separados por comas `(parameter1, parameter2)`.

El cuerpo de la función debe sangrar cuatro espacios. Si no hay ningún código para que la función se ejecute, un `pass` debe incluirse en la definición de la función.

```don
def my_function():
    pass
```

## Ejemplo 1

Esta función no tiene parámetros e imprimirá "Hello" en la pantalla del V5 Brain.

```don
def print_hello_world():
    brain.screen.print("Hello World")
```
## Ejemplo 2

Esta función toma un parámetro, `name` e imprimirá el valor de `name` en la pantalla del V5 Brain.

```don
def print_name(name):
    brain.screen.print(name)
```

<advanced>
</advanced>
