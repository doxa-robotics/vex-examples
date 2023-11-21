category: drivetrain
signature: drivetrain.set_stopping(BRAKE)
description: Sets the behavior of the robot once it stops moving.  

# Establecer Detención

`drivetrain.set_stopping(MODE)` establece el comportamiento del robot cuando deja de moverse.  

## Cómo Utilizar

Sustituya el parámetro 'MODE' por una de las siguientes opciones:

* BRAKE (Freno): hará que el Motor se detenga inmediatamente.
* COAST (Costa): deja que el Motor gire gradualmente hasta detenerse.
* HOLD (Detener): hará que el robot se detenga inmediatamente y lo devuelve a su posición de parada si se mueve. La parada del robot establecido surtirá efecto para todos los comandos futuros del robot para el resto del proyecto.

## Ejemplo

Este ejemplo muestra el robot conduciendo hacia adelante durante 200 MM antes de conducir por inercia hasta detenerse.

```don
drivetrain.set_stopping(COAST)
drivetrain.drive_for(FORWARD, 200, MM)
```
<advanced>
</advanced>
