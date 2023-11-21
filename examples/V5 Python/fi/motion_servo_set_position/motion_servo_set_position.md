category: motion  
signature: servo.set_position(50, DEGREES)  
description: Sets the Servo's encoder position to the given value.

# Pyöritä Servo -moottoria

Pyörittäa Servo -moottoria tiettyyn asentoon.

```python
servo.set_position(POSITION, DEGREES)
```

## Miten käytetään

`servo.set_position()` komento sallii arvot **-50** - **50** parametrin **POSITION** arvoksi.

## Esimerkki

Alla moottori pyörii asentoon 25 astetta ja odottaa 2 s ja sitten asentoon -25 astetta.

```python
servo.set_position(25, DEGREES)
wait(2, SECONDS)
servo.set_position(-25, DEGREES)
```

<advanced>
</advanced>
