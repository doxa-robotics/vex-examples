category: motion  
signature: motor.set_max_torque(50, PERCENT)  
description: Sets the strength of the V5 Smart Motor.  

# Ajuste de la Par del Motor

Establece el par del V5 Smart Motor.

```don
motor.set_max_torque(AMOUNT, PERCENT)
```

## Cómo Utilizar

Este comando acepta un rango de 0% a 100%.

El comando "set motor torque" puede aceptar decimales, enteros o valores numéricos

## Ejemplo

Este ejemplo girará el motor de garra a la posición de 40 grados con sólo un 20% de par máximo. Esto permite que la garra agarre un objeto sin dañarlo con demasiada fuerza.

```don
claw_motor.set_max_torque(20, PERCENT)
claw_motor.set_position(40, DEGREES)
```

<advanced>
</advanced>
