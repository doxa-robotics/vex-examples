category: motion  
signature: SERVO.setPosition(90, degrees);  
device_class: servo
description: Spins a V5 Servo Motor to a set position.  

# Servo Set Position

Pyörittää V5 Servo Mooottoria tiettyyn asentoon.

```cpp
Servo.setPosition(position, degrees);
```

## Miten käytetään

Pyörittää servomoottoria tiettyyn asentooon.

`Servo.setPosition()` komento hyväksyy arvot välillä **-50** - **50** parametrissa **position**.


## Esimerkki

Esimerkissä servomoottori pyörii asentoon 25 astetta ja odottaa 2 sekuntia ja pyörii vielä asentoon -25 astetta.

```cpp
Servo.setPosition(25, degrees);
wait(2, seconds);
Servo.setPosition(-25, degrees);
```

<advanced>
</advanced>