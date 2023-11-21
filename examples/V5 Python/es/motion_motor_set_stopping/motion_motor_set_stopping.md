category: motion  
signature: motor.set_stopping(BRAKE)  
description: Sets the behavior of the V5 Smart Motor once it stops moving.

# Establecer Parada del Motor

Establece el comportamiento de frenado del V5 Smart Motor.

```don
motor.set_stopping(MODE)
```

## Cómo Utilizar

El parámetro `MODE` se puede sustituir por cualquiera de las siguientes opciones:

* BRAKE (Frenar): hará que el motor se detenga inmediatamente.
* COAST (Deslizarse): deja que el motor gire gradualmente hasta detenerse.
* HOLD (Detener): will cause the Motor to come to an immediate stop, and returns it to its stopped position if moved.

El comportamiento de detención establecido por este comando se aplicará a los comandos de motor subsiguientes para la totalidad del proyecto, a menos que se cambie de otra manera.

## Ejemplo

Este ejemplo hará que el Motor de brazo gire hacia adelante durante 90 grados (para levantar el brazo) y luego mantendrá su posición.

```don
arm_motor.set_stopping(HOLD)
arm_motor.spin_for(FORWARD, 90, DEGREES)
```

<advanced>
</advanced>
