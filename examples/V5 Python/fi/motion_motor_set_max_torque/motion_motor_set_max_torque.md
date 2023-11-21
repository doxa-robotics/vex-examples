category: motion  
signature: motor.set_max_torque(50, PERCENT)  
description: Sets the strength of the V5 Smart Motor.  

# Aseta maksimi moottorin vääntö

Asettaa V5 älymoottorin masimi väännön.

```don
motor.set_max_torque(AMOUNT, PERCENT)
```

## Miten käytetään

Komento sallii arvot välillä 0% - 100%.

Maksimi moottorin vääntö -komento sallii desimaali- ja kokonaislukuja sekä numeerisia arvoja.

## Esimerkki

Esimerkissä kouramoottori liikkuu asentoon 40 astetta maksimi moottorin väännöllä 20 %, jolloin tarttuessa esineeseen moottori ei riko esinettä.

```don
claw_motor.set_max_torque(20, PERCENT)
claw_motor.set_position(40, DEGREES)
```

<advanced>
</advanced>
