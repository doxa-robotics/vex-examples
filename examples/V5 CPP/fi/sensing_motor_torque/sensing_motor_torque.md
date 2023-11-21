category: sensing  
signature: MOTOR.torque()  
device_class: motor  
description: Reports the amount of torque (rotational force) a V5 Smart Motor is currently using.

# Moottorin vääntövoima

Antaa V5 Älymoottorin vääntövoiman (kiertovoiman) tällähetkellä.

```cpp
Motor.torque(Nm)
```

## Miten käytetään

`Motor.torque()` antaa desimaaliarvon (muotoa *double*) vääntövoimalle tällä hetkellä.

Komentoa voi käyttää muiden komentojen argumenttina mm tulostuksessa tai erikseen toistorakenteiden vertailuehdoissa.

Komento antaa arvot välillä **0.0 - 2.1 Newton-metriä (Nm)**.

```cpp
Brain.Screen.print("%f", ArmMotor.torque(Nm));
```

VToinen yksikkö on tuuma-paunaa (`InLb`) ja sen mittaväli on **0.0 - 18.6 InLb**. 

```cpp
Brain.Screen.print("%f", ArmMotor.torque(InLb));
```
<advanced>
</advanced>