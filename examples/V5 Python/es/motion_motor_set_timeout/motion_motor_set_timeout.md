category: motion  
signature: motor.set_timeout(1, SECONDS)  
description: Sets a time limit for the V5 Smart Motor movement commands.

# Establecer Tiempo de Espera del Motor

Establece un límite de tiempo para los comandos de movimiento del V5 Smart Motor.

```don 
motor.set_timeout(AMOUNT, SECONDS)
```

## Cómo Utilizar

El límite de tiempo del motor se utiliza para evitar que los comandos de movimiento que no alcanzan su posición impidan que los comandos subsiguientes se ejecuten. 

Un ejemplo de que un motor no alcanza su posición es un brazo o una garra que alcanza su límite mecánico y no puede completar su movimiento.

El comando `set_motor_timeout` puede aceptar decimales, enteros o valores numéricos.

## Ejemplo

Este ejemplo finalizará el comando SET motor después de 2 segundos si el motor de claw no ha alcanzado la posición de 270 grados. Una vez alcanzado el límite de tiempo o el objetivo, el motor de claw girará a la posición 0 grados.

```don
claw_motor.set_timeout(2, SECONDS)
claw_motor.spin_to_position(270, DEGREES)
claw_motor.spin_to_position(0, DEGREES)
```

<advanced>
</advanced>
