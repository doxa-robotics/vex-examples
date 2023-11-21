category: control  
signature: while expression: \n\tpass  
description: A loop that repeats the code while the condition returns true. 

# Mientras
Bucle que repite el código en su cuerpo siempre que la expresión de condición se evalúe como **true**.   

```don
while condition:
   pass
```

## Cómo Utilizar

El bucle 'while' solo comprobará la condición dentro del paréntesis al principio de cada bucle. 

Si la condición se evalúa como **true**, el código dentro de 'while' se ejecutará.

Si la condición se evalúa como **false**, el código dentro de 'while' se omitirá.

El bucle 'while' acepta todo lo que se evalúa como 'True' o 'False' como su condición. Puede colocar booleanos, así como expresiones, utilizando operadores de comparación y lógicos. 

También puede utilizar valores numéricos; *0** se evalúa como 'False', y cualquier **número distinto de cero** se evalúa como 'True'.

Agregue una sangría de cuatro espacios usando la **barra espaciadora** para incluir declaraciones como parte de la declaración de control 'while'. 

Una instrucción 'while' no debe contener un bloque vacío de código. Si es necesario, agregue una instrucción 'pasa' a una instrucción 'while' previamente vacía. 

## Ejemplo

Este bucle 'while' seguirá imprimiendo la palabra "Hello" en líneas separadas cuando el valor del temporizador sea inferior a 50 segundos.

```don
while brain.timer.time(SECONDS) < 50:
    brain.screen.print("Hello")
    brain.screen.new_line()
```

<advanced>
</advanced>
