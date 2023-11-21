category: control  
signature: if condition:\n\tpass  
description: Used to decide whether or not a statement will be executed  

# Si

Una declaración de control utilizada para decidir si un bloque de código se ejecutará en función de la 'condition' proporcionada.

```don
if condition:
    pass
    
```

## Cómo Utilizar

Reemplace la palabra 'condition' por una expresión que pueda evaluarse como 'True' o 'False`. Una evaluación de 'True' permitirá que las instrucciones indentadas debajo de la instrucción 'if' se ejecuten.

Agregue una sangría de cuatro espacios usando la **barra espaciadora** para incluir declaraciones como parte de la declaración de control 'if'. 

Una declaración 'if' no debe contener un bloque de código vacío. Si es necesario, añadir una declaración 'pass' a una declaración 'if' previamente vacía. 

## Ejemplo

Esta instrucción 'if' se ejecutará si 'my_variable' es igual a 1, haciendo que el robot conduzca hacia adelante.

```don
if (my_variable == 1):
    drivetrain.drive(FORWARD)
```

<advanced>
</advanced>
