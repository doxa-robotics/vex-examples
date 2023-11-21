category: motion  
signature: motor.stop()  
description: Stops a motor.

# Detener el motor

Detiene el motor.

```don
motor.stop()
```

## Ejemplo

Este ejemplo muestra un motor girando durante 3 segundos antes de detenerse.

```don
motor.spin(FORWARD)
wait(3, SECONDS)
motor.stop()
```

<advanced>
</advanced>
