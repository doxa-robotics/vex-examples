category: sensing  
signature: brain.timer.clear()  
description: Clears the V5 Brain's timer.

# Restablecer Temporizador
Restablece el temporizador del V5 Brain.

```don 
brain.timer.clear()
```

## Cómo Utilizar

El temporizador del V5 Brain comienza al principio de cada proyecto. El comando CLEAR TIMER restablece el valor del temporizador a 0 segundos.

## Ejemplo

En este ejemplo, el temporizador se reiniciará antes de mover el Chasis hacia adelante durante 3 segundos. Después de 3 segundos, el Chasis se detendrá.

```don
brain.timer.clear()
while not brain.timer.time(SECONDS) > 3:
    drivetrain.drive(FORWARD)
drivetrain.stop()
```
	
<advanced>
</advanced>
