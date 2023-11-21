category: drivetrain 
signature: drivetrain.turn_to_heading(90, DEGREES)  
description: Turns a Drivetrain to a specific heading, when using the Gyro or Inertial sensors.

# Dar Vuelta a la Dirección

Gira el chasis a una dirección específica cuando se utilizan los sensores Gyro o Inertial.

`drivetrain.turn_to_heading(HEADING, UNITS)`

## Cómo Utilizar

El comando `drivetrain.turn_to_heading` se puede utilizar para girar el chasis a cualquier dirección dado en el sentido de las agujas del reloj.

Basado en la dirección actual del Giroscopio, `drivetrain.turn_to_heading` determinará la dirección a girar.

El parámetro `HEADING` acepta valores numéricos en el rango de **0.00 a 359.99**.

El parámetro `UNITS` (unidades) debe establecerse en `DEGREES`(grados).

## Ejemplo

Este ejemplo hará que el chasis haga cuatro vueltas: 

```don
drivetrain.turn_to_heading(45.0, DEGREES)
drivetrain.turn_to_heading(90.0, DEGREES)
drivetrain.turn_to_heading(270.0, DEGREES)
drivetrain.turn_to_heading(180.0, DEGREES)
```

- Left to 45 degrees (Izquierda a 45 grados)
- Left to 90 degrees (Izquierda a 90 grados)
- Left to 270 degrees (Derecha a 270 grados)
- Right to 180 degrees (Derecha a 180 grados)

El comando `turn_to_heading` por defecto bloqueará los comandos de procedimiento hasta que el giro del chasis se haya completado.

## Parámetros Optionales

Puede establecer `wait=False` como tercer parámetro para prevenir el comando `turn_to_heading` de bloquear los comandos de procedimiento de ejecución hasta que el giro del chasis se haya completado.

```don
drivetrain.turn_to_heading(180.0, DEGREES, wait=False)
```

<advanced>
</advanced>
