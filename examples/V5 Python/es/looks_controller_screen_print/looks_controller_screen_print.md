category: looks  
signature: controller.screen.print("Hello World")  
description: Prints values or text on the V5 Controller's screen.  

# Imprimir

Imprime valores en la pantalla del V5 Controller.

```don
controller.screen.print("Hello World") 
```

## Cómo Utilizar

El comando `controller.screen.print()` imprimirá los datos en la posición del cursor en la pantalla.

Todos los nuevos proyectos comienzan con el cursor de la pantalla en la fila 1, columna 1.


* Imprimir palabras y números: 
	`controller.screen.print("Number:", 10)`
* Imprimir el valor informado de una variable:  
	`controller.screen.print(my_variable)`
* Imprime el valor notificado desde un sensor o dispositivo: 
        `controller.screen.print(drivetrain.is_done())`
	
<advanced>
</advanced>
