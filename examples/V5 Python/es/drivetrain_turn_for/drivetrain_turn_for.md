category: drive  
signature: drivetrain.turn_for(RIGHT, 90, DEGREES, wait=True) 
description: Turns the Drivetrain for a given distance.  

# Dar Vuelta Por

Gira el chasis durante un número especificado de grados.

```don
drivetrain.turn_for(DIRECTION, ANGLE, UNITS)
```

## Cómo Utilizar

El primer argumento especifica la dirección de giro: 'LEFT' (izquierda) o 'RIGHT' (derecha), escrita en letras mayúsculas. 

El segundo argumento especifica el ángulo de giro como un valor numérico; puede ser cualquier número entre 0 y 360. 

El tercer argumento son las unidades de giro. Esto debe ser establecido como "DEGREES" en letras mayúsculas. 

El comando 'turn_for' es de forma predeterminada un comando de bloqueo. Impide que se ejecute cualquier código hasta que el chasis haya completado su turno.

## Parámetros Opcionales

Si el cuarto argumento se establece en 'wait=False', comandos de procedimiento se les permitirá ejecutar incluso antes de que el chasis ha completado su turno.

```don
drivetrain.turn_for(LEFT, 90, DEGREES, wait=False)
```

## Ejemplo

Este ejemplo girará el V5 Robot 270 grados a la derecha.

```don
drivetrain.turn_for(RIGHT, 270, DEGREES)
```

<advanced>
</advanced>
