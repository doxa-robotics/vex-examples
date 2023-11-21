category: drivetrain
signature: drivetrain.set_heading(0, DEGREES)  
description: Sets the Gyro of the Drivetrain to an exact heading.  

# Establecer Dirección del Chasis

Establece el Gyro del chasis en una dirección exacto.

```don
drivetrain.set_heading(HEADING, UNITS)
```

## Cómo Utilizar

El comando 'drivetrain.set_heading' se puede utilizar para establecer la posición de la chasis en cualquier dirección dado. Este comando se puede utilizar para restablecer la orientación del giroscopio del chasis cuando le dirección se establece en un valor de 0.

`drivetrain.set_heading` acepta un valor numérico entre **0 y 360** ya que es el primer argumento, y 'DEGREES' escrito en letras mayúsculas como su segundo argumento.

## Ejemplo

En este ejemplo se establece el rumbo de la transmisión a 90 grados. 

Dado que la dirección del V5 Robot se establece en 90 grados, el siguiente comando 'turn_to_heading' no hará que el robot gire ya que su encabezado actual ya se ha establecido en 90 grados.

```don
drivetrain.set_heading(90, DEGREES)
drivetrain.turn_to_heading(90, DEGREES)
```

<advanced>
</advanced>
