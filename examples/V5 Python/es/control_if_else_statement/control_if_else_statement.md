category: control  
signature: if condition: \n\tpass\nelse:\n\tpass  
description: Used to decide if one statement will execute or another will if the first statement is not true.

# Si/Si no
Una instrucción de flujo de control que ejecuta un bloque de comandos si una condición se evalúa como true, u otro bloque de comandos si una condición se evalúa como false. 

```don
if condition:
    pass
else:
    pass

```

## Cómo Utilizar

La instrucción 'if' es un condicional que comprobará si su condición se evalúa como **True** o **False**. Es posible combinar muchas condiciones con el uso de operadores lógicos como 'and', 'or' y 'not`. 

Si la totalidad de la condición es **True**, entonces el bloque de código indentado debajo de la 'condición if': se ejecutará. Si la totalidad de la condición es **False**, el bloque de código con sangría debajo de la instrucción 'else:' se ejecutará en su lugar.

Los bloques de código por debajo de 'if' y 'else' deben sangrar cuatro espacios.

Una declaración `if/else` no debe contener bloques de código vacíos. Si es necesario, añada las declaraciones 'pass' a una declaración 'if/else' vacía anteriormente. 

## Ejemplo

El codigo `if/else` Accionará el robot FORWARD si la variable es igual a 1. Si no, conducirá el robot REVERSE. 

```don
if (my_variable == 1):
    drivetrain.drive(FORWARD)
else:
    drivetrain.drive(REVERSE)
```

<advanced>
</advanced>
