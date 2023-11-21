category: motion  
signature: motor.set_velocity(50, PERCENT)  
description: Sets the speed of a V5 Smart Motor.

# Establecer la Velocidad del Motor

Establece la velocidad de un V5 Smart Motor.


```don 
motor.set_velocity(VELOCITY, UNIT)
```

## Cómo Utilizar

Este comando acepta un rango de **-100% a 100%** o **-600rpm a 600rpm.**

El valor 'UNIT' (Unidad) aceptable es: `PERCENT` (Por Ciento) or `RPM` (Rotación por Minuto) .

**Ajuste la velocidad del motor** aceptará un valor de "rotaciones por minuto" (RPM) basado en el cartucho de engranaje instalado en los V5 Smart Motor.

* Red Cartridge (Cartucho de Engranaje Rojo): -100rpm a 100rpm
* Green Cartridge (Cartucho de Engranaje Verde): -200rpm a 200rpm
* Blue Cartridge (Cartucho de Engranaje Azul): -600rpm a 600rpm

Si se establece la velocidad de un V5 Smart Motor en un valor negativo, el motor girará en sentido inverso.

Si se establece la velocidad de un V5 Smart Motor en 0, se evitará que el motor gire.

## Ejemplo

Este ejemplo establecerá que el Motor de brazo gire a una velocidad del 25% a la posición de 90 grados.

```don
arm_motor.set_velocity(25, PERCENT)
arm_motor.spin_to_position(90, DEGREES)
```

<advanced>
</advanced>
