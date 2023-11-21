category: sensing  
signature: inertial.set_heading(0, DEGREES)
description: Sets the Inertial sensor's current heading position to a set value.

# Establecer Dirección del Inercial

Establece la dirección actual del Sensor Inercial en un valor establecido.

```don
inertial.set_heading(HEADING, DEGREES)
```

## Cómo Utilizar

`inertial.set_heading` se puede utilizar para establecer la posición del giroscopio en cualquier dirección en el sentido de las agujas del reloj. Este comando se utiliza normalmente para restablecer la orientación del Sensor Inercial cuando la dirección se establece en un valor de 0.

`inertial.set_heading` Se utiliza normalmente para restablecer la orientación de la dirección del Sensor Inercial cuando un valor se establece en 0.

`inertial.set_heading` acepta un rango de 0.0 a 359.99 grados.

`inertial.set_heading` pueden aceptar decimales, enteros o valores numéricos.


<advanced>
</advanced>
