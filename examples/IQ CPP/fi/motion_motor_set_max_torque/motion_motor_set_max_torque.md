category: motion  
signature: Motor.setMaxTorque(50, percent);
device_class: motor  
description: Sets the Motor's max torque.  

# Moottori Max vääntövoima

Asettaa moottorin maksimi vääntövoiman.  

```cpp
Motor.setMaxTorque(value, percent);
```

## Miten käytetään

`Motor.setMaxTorque` hyväksyy arvot välillä **0% - 100%**.

Komennon ensimmäinen osa on moottorin nimi.

```cpp
ClawMotor.setMaxTorque(25, percent);
ArmMotor.setMaxTorque(75, percent);
```

## Esimerkki

Esimerkissä kouramoottori ClawMotor pyörii asentoon 40 astetta vain 20% maksimi väännöllä. Tällöin säästytään turhalta voimankäytöltä ja puristukseltaa, kun esine otetaan kiinni kouraan.

```cpp
ClawMotor.setMaxTorque(20, percent);
ClawMotor.spinToPosition(40, degrees);
```

<advanced>
</advanced>