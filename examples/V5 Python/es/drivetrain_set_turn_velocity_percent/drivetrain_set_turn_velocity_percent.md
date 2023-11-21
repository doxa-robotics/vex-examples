category: drivetrain
signature: drivetrain.set_turn_velocity(50, PERCENT)  
description: Sets the Drivetrain's turn velocity.

# Establecer la Velocidad de Dar Vuelta

Establece la velocidad de veuletas del chasis.

```don
drivetrain.set_turn_velocity(VELOCITY, PERCENT)
```

## Cómo Utilizar

`drivetrain.set_turn_velocity` establecerá la velocidad del chasis al girar, pero no hará que el chasis se mueva cuando se usa sin un comando de 'turn' o 'turn_for'.

`drivetrain.set_turn_velocity` acepta un rango de **-100 a 100** como primer argumento. Toma las unidades, `PERCENT`, escrito en letras mayúsculas como el segundo argumento.

Establecer la velocidad de vuelta del chasis en un valor negativo hará que el chasis gire en el opuesto de la dirección pasada en los siguientes comandos de giro.

Establecer la velocidad de giro del chasis en 0 evitará que el chasis gire, incluso cuando se utiliza un comando 'turn' o 'turn_for'.

## Ejemplo

En este ejemplo, el chasis girará en la dirección opuesta debido a un valor negativo.

```don
drivetrain.set_turn_velocity(-100, PERCENT)
drivetrain.turn(RIGHT)
```


<advanced>
</advanced>
