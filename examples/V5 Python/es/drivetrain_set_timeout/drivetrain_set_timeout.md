category: drivetrain
signature: drivetrain.set_timeout(1, SECONDS)
description: Sets a time limit for the robot movement commands.

# Establecer Tiempo de Espera

`drivetrain.set_timeout(VALUE, SECONDS)` establece un límite de tiempo para los comandos de movimiento del robot.

## Cómo Utilizar

El comando se utiliza para evitar que los comandos de movimiento que no alcanzan su posición impidan que otros comandos de procedimiento se ejecuten.

El comando puede aceptar valores numéricos o decimales.

## Ejemplo

Este ejemplo muestra un tiempo de espera que se utiliza para establecer el límite de tiempo para los movimientos de avance del chasis.

```don
drivetrain.set_timeout(1, SECONDS)
drivetrain.drive_for(FORWARD, 100, MM)
drivetrain.drive_for(FORWARD, 200, MM)
```

<advanced>
</advanced>
