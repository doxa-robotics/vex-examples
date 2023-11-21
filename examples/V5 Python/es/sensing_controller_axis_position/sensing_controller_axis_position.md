category: sensing  
signature: controller.axis1.position()  
description: Reports the position of a joystick on the V5 Controller along an axis.

# Posición del Controller
 
Reporta la posición de un joystick en el V5 Controller a lo largo de un eje.

```don
controller.axis1.position()
```

## Cómo Utilizar

`controller.axis1.position` reporta de un rango entre **-100 a 100**.

`controller.axis1.position` informará cero (0) cuando un eje de joystick esté centrado.

Elija qué eje del controlador debe informar.

* axis1 (eje 1) - Joystick derecho (izquierda y derecha)
* axis2 (eje 2)- Joystick derecho (arriba y abajo)
* axis3 (eje 3)- Joystick izquierdo (arriba y abajo)
* axis4 (eje 4)- Joystick izquierdo (izquierda y derecha)
	
<advanced>
</advanced>
