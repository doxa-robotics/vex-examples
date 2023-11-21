category: drivetrain 
signature: drivetrain.turn(RIGHT)  
description: Turns the Drivetrain to the right or left.  

# Dar Vuelta

Hara que el chasis de vuelta a la derecha o a la izquierda.

```don
drivetrain.turn(DIRECTION)
```

## Cómo Utilizar

El comando "drivetrain.turn" girará el Drivetrain en la dirección dada por siempre hasta que se utilice un nuevo comando drivetrain, o hasta que se detenga el programa.

Utilice el argumento 'LEFT' en letras mayúsculas para girar el chasis a la izquierda.

```don
drivetrain.turn(LEFT)
```

Utilice el argumento 'RIGHT' en letras mayúsculas para girar el chasis a la derecha.

```don
drivetrain.turn(RIGHT)
```

## Ejemplo

En esta ejemplo, el robot avanzará 200 MM antes de girar a la derecha indefinidamente.

```don
drivetrain.drive_for(FORWARD, 200, MM)

drivetrain.turn(RIGHT)
```

<advanced>
</advanced>
