category: control  
signature: for value in range (10): \n\tpass  
description: A type of loop that repeats the code contained inside for a set number of iterations. 

# Por

Un tipo de bucle que repite el código contenido en su cuerpo para un número determinado de iteraciones.

```don
for value in range(10):
    pass
```

# Cómo Utilizar

Primero, reemplace 'value' por una variable que se iterará a través de la función 'range()'.

En segundo lugar, sustituya '10' por un valor para especificar el final de la iteración.

Agregue una sangría de cuatro espacios usando la barra espaciadora para incluir declaraciones como parte de la instrucción de control 'for'.

Una declaración 'for' no debe contener un bloque de código vacío. Si es necesario, añada una declaración 'pass' a una declaración de for previamente vacía.

Observe que los bucles for comienzan en el índice 0 en lugar de 1.

Los bucles 'for' también pueden anidarse entre sí.

# Ejemplo
El siguiente bucle for imprimirá los números 0 a 2:

```don
for i in range(3):
   brain.screen.print(i)
   brain.screen.new_line()
```
   
Esto imprimirá:

```
0
1
2
```

<advanced>
</advanced>
