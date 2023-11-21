category: motion  
signature: MOTOR.setPosition(0, degrees);  
device_class: motor  
description: Sets the V5 Smart Motor's encoder to a position.  

# Moottorin asennon asetus

Asettaa V5 Älymoottorin kierrosmittarille (encoder) arvon.

```cpp
Motor.setPosition(position, units);
```

## Miten käytetään

`Motor.setPosition();` komennolle voi asettaa V5 Älymoottorin kierrosmittarille (encoder) halutun arvon.

`Motor.setPosition();` komentoa käytetään tyypillisesti, kun nollataan asento.

Voit käyttää 'position` arvona mitä tahansa numeroa. 

Yksikkönä voi käyttää joko `degrees`(astetta) tai `turns` (kierroksia). 

```cpp
ArmMotor.setPosition(50, degrees);
```

<advanced>
</advanced>