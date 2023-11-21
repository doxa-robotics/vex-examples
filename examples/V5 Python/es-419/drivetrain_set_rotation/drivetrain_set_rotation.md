category: drivetrain
signature: drivetrain.set_rotation(0, DEGREES)  
description: Sets the Drivetrain's angle of rotation with a Gyro Sensor.

# Establecer Rotación

Establece el ángulo de rotación del chasis con un sensor Gyro.

```don
drivetrain.set_rotation(ROTATION, UNITS)
```

## Cómo Utilizar

El comando 'drivetrain.set_rotation' se puede utilizar para establecer el ángulo de rotación del chasis a cualquier valor positivo o negativo dado.

El parámetro 'ROTATION' puede aceptar valores numéricos.

El parámetro 'ROTATION' **no** tiene un límite de 0-359 grados.

## Ejemplo

Este ejemplo hará girar el robot un total de 210 grados:

```don
drivetrain.turn_to_rotation(120, DEGREES)
drivetrain.set_rotation(-45, DEGREES)
drivetrain.turn_to_rotation(45, DEGREES)
```

- Turn right (clockwise) to rotation 120 degrees.
- Set the robot's current position as rotation of -45 degrees.
- Turn right (clockwise) an additional 90 degrees (-45 degrees to +45 degrees) based on the set rotation value from the previous command.

<advanced>
</advanced>
