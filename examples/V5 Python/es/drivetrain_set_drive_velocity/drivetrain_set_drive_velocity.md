category: drivetrain  
signature: drivetrain.set_drive_velocity(50, PRECENT)  
description: Sets the velocity of the Drivetrain that will be used for drive() and drive_for() commands.

# Establecer Velocidad de Conducción

Establece la velocidad del chasis para los comandos 'drive' y 'drive_for'. La velocidad predeterminada es 50%. 

```don
drivetrain.set_drive_velocity(VELOCITY, PERCENT)
```

## Cómo Utilizar

`drivetrain.set_drive_velocity` establecerá la velocidad del chasis cuando se utiliza con un comando 'drive' o 'drive_for'. No hará que el chasis se mueva cuando se utiliza por sí mismo.

`drivetrain.set_drive_velocity` acepta dos argumentos: un valor numérico de **-100  to 100**, y el argumento de la unidad 'PERCENT' escrito en letras mayúsculas. 

Si se establece la velocidad del chasis en un valor negativo, el chasis se encontrará en el lado opuesto de la 'DIRECTION' pasada a un comando 'Drive' o 'Drive_for'.

Si se establece la velocidad del chasis en 0, se evitará que el chasis se mueva incluso si se utiliza un comando 'Drive' o 'Drive_for'.

## Ejemplo

Este ejemplo muestra que el chasis irá en reversa debido a un valor negativo.

```don
drivetrain.set_drive_velocity(-100, PERCENT)
drivetrain.drive(FORWARD)
```

Este ejemplo evitará que el chasis se mueva.

```don
drivetrain.set_drive_velocity(0, PERCENT)
drivetrain.drive(FORWARD)
```

<advanced>
</advanced>
