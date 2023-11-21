category: drive  
signature: drivetrain.drive(FOWARD)  
description: Moves the Drivetrain forever in the direction specified inside of the parentheses. 

# Conducir

Mueve el chasis por siempre en la dirección especificada dentro de los paréntesis. 

Todos los motores del chasis funcionan hacia adelante o hacia atrás a la velocidad establecida mediante el comando 'drivetrain.set_drive_velocity'. La velocidad predeterminada es 50%. 

Los valores negativos harán que el chasis conduzca hacia atrás con una entrada REVERSE y en hacia adelante con una entrada FORWARD.

```don
drivetrain.drive(DIRECTION)
```

## Cómo Utilizar

El comando 'drivetrain.drive' ejecutará el chasis para siempre, hasta que se utilice un nuevo comando drivetrain, o el programa se detenga.

## Ejemplos

Utilice el argumento 'FORWARD' en las letras mayúsculas para mover el chasis hacia adelante.

```don
drivetrain.drive(FORWARD)
```

Utilice el argumento 'REVERSE' en las letras mayúsculas para mover la transmisión en sentido inverso.

```don
drivetrain.drive(REVERSE)
```
 
<advanced>
</advanced>
