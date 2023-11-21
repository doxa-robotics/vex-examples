category: control  
signature: while not expression: \n\tpass  
description: A loop that continues until the expression turns true.  

# Mientras no
Instrucción de control que continúa realizando bucles hasta que se convierte la expresión **true**.

```don
while not condition:
    pass
```

## Cómo Uilizar

Cómo la declaración 'while not' comprobará repetidamente la condición, y no pasará al siguiente comando hasta que la condición indique **true**.

Si la condición se evalúa como **false**, el código dentro de 'while not' se ejecutará.

Si la condición se evalúa como **true**, el código dentro de 'while not' se omitirá, y el siguiente comando después de la instrucción 'while not' se ejecutará.

La declaración de 'while not' acepta cualquier expresión que se evalúe como 'True' o 'False' como su condición. Puede colocar booleanos, así como expresiones, utilizando operadores de comparación y lógicos. 

También puede utilizar valores numéricos; **0** evalúa a 'False`, Y cualquier **número distinto de cero** se evalúa como 'True`. 

Agregue una sangría de cuatro espacios usando la **barra espaciadora** para incluir declaraciones como parte de la declaración de control 'while not'. 

Una declaración de 'while not' no debe contener un bloque de código vacío. Si es necesario, añadir una declaración 'pasa' a una declaración 'while not' vacía. 

## Ejemplo

Este bucle 'while not' imprimirá "Hello" en líneas separadas hasta que el valor de mi variable sea igual a 5.

myVariable = 0

```
while not my_variable == 5:
    brain.screen.print("Hello")
    brain.screen.new_line()
    my_variable += 1
```

<advanced>
</advanced>
