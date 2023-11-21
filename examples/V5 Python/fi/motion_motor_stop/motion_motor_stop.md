category: motion  
signature: motor.stop()  
description: Stops a motor.

# Pysäytä moottori

Pysäyttää moottorin.

```don
motor.stop()
```

## Esimerkki

Esimerkissä moottori pyörii 3 sekuntia ennen pysähtymistä.

```don
motor.spin(FORWARD)
wait(3, SECONDS)
motor.stop()
```

<advanced>
</advanced>
