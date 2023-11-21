category: looks  
signature: brain.screen.print("Hello World")  
description: Prints values or text on the V5 Brain's screen.  

# Imprimir

Imprime valores o texto en la pantalla del V5 Brain.

```don
brain.screen.print("Hello World")
```

## Cómo Utilizar

El comando `brain.screen.print()` imprimirá datos en una ubicación del cursor en la pantalla.

Todos los nuevos proyectos comienzan con el cursor de la pantalla en la fila 1 columna 1.


* Print words and numbers: 
	`brain.screen.print("Number:", 10)`
* Print the reported value from a variable: 
	`brain.screen.print(my_variable)`
* Print the reported value from a sensor or device:  
        `brain.screen.print(drivetrain.is_done())`



<advanced>
</advanced>
