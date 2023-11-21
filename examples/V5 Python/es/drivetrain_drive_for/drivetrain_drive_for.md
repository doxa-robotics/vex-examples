category: drivetrain 
signature: drivetrain.drive_for(FORWARD, 2, MM, wait=True)
description: Moves the Drivetrain for a given distance.  

# Conducir Por

Mueve el chasis por una distancia determinada. Todos los motores del chasis funcionan hacia adelante o hacia atrás a la velocidad establecida por el comando 'drivetrain.set_drive_velocity'. Después de que el chasis haya movido la distancia de entrada, el chasis se detendrá.

```don
drivetrain.drive_for(DIRECTION, DISTANCE, UNITS)
```

## Cómo Utilizar

Establezca la distancia a la que se moverá el chasis introduciendo al menos tres argumentos válidos dentro de los paréntesis, separados por comas. 

El primer argumento especifica la dirección. Las entradas válidas son 'FORWARD' o 'REVERSE' en todas las letras mayúsculas.  

El segundo argumento especifica la distancia que debe conducir el V5 Robot.

El tercer argumento especifica la unidad de medida que debe usarse. Las entradas válidas son 'INCHES'(pulgadas) o 'MM' (milímetros) en letras mayúsculas.

El parámetro 'DISTANCE' acepta valores numéricos. Los valores negativos harán que el robot V5 conduzca en sentido contrario a la entrada 'DIRECTION'.

```
drivetrain.drive_for(REVERSE, 5.0, INCHES)
```

El comando "drive_for" es por defecto un comando de bloqueo. Evitará que se ejecuten comandos posteriores hasta que se haya completado el movimiento de chasis.

## Parámetro opcional

Puede establecer un cuarto parámetro en 'wait=False' para permitir que los comandos que se siguen se ejecuten incluso antes de que el chasis haya terminado de moverse.

```don
drivetrain.drive_for(FORWARD, 200, MM, wait=False)
```

## Ejemplo

Este ejemplo muestra el 'drivetrain.drive_for' que se utiliza con una variable como distancia.

El V5 Robot se conduce 200 MM hacia adelante.

```don
distance_variable = 200

drivetrain.drive_for(FORWARD, distance_variable, MM)
```

<advanced>
</advanced>
