category: drivetrain
signature: drivetrain.turn_to_rotation(90, DEGREES, wait=True)
description: Turns the Drivetrain to a specific angle of rotation..  

# Dar vuelta a la Rotación

Gira el chasis a un ángulo de rotación específico.

`drivetrain.turn_to_rotation(ROTATION, DEGREES)`

## Cómo Utilizar

El comando `drivetrain.turn_to_rotation` se puede utilizar para girar el chasis a un valor positivo (en el sentido de las agujas del reloj) o negativo (en sentido contrario a las agujas del reloj).

Basado en la rotación actual del chasis, `drivetrain.turn_to_rotation` determinará la dirección a girar.

El parámetro `ROTATION` puede aceptar valores numéricos.

Los valores numéricos **no** son limitados al rango de **0 - 359.99** grados. Los giros serán absolutos y pueden hacer que el robot gire más de una vez si es necesario.

## Ejemplo

Este ejemplo hará que el chasis haga cuatro vueltas:

```don
drivetrain.turn_to_rotation(90.0, DEGREES)
drivetrain.turn_to_rotation(180, DEGREES)
drivetrain.turn_to_rotation(-45, DEGREES)
drivetrain.turn_to_rotation(0, DEGREES)
```

- Right (Derecha (en el sentido de las agujas del reloj)) a 90 grados
- Right(Derecha (en el sentido de las agujas del reloj)) a 180 grados
- Left (Izquierda (en sentido opuesto al de las agujas del reloj)) a -45 grados
- Right (Derecha(en el sentido de las agujas del reloj)) a 0 grados

El comando `drivetrain.turn_to_rotation` por defecto bloqueará los comandos de procedimiento hasta que el giro del chasis se haya completado.

## Parámetro opcional

Puede establecer un tercer parámetro  `wait=False` para evitar el comando `turn_to_rotation' de bloquear los comandos de procedimiento hasta que se complete el giro del chasis.

```don
drivetrain.turn_to_rotation(180.0, DEGREES, wait=False)
```

<advanced>
</advanced>
