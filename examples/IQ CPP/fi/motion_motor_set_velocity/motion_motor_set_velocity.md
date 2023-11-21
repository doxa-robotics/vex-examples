category: motion  
signature: Motor.setVelocity(50, percent);  
device_class: motor  
description: Sets the Motor's velocity.  

# Aseta Moottorin Nopeus

Asettaa VEX IQ Älymoottorin nopeuden.

```cpp
Motor.setVelocity(velocity, units);
```

## Miten käytetään

`Motor.setVelocity` hyväksyy arvot **-100% - 100%** tai **-127rpm - 127rpm**.

Jos antaa nopeudelle negatiivisen arvon, moottori pyörii oletetusta taaksepäin.

Jos asetaa nopeudella arvon 0 , moottori pysähtyy.

Komennon ensimmäinen osa on halutun moottorin nimi.

```cpp
ClawMotor.setVelocity(25, percent);
ArmMotor.setVelocity(75, percent);
```

Nopeuden yksikkö on joko **percent** (prosentti) tai **rpm** (kierrosta minuutissa).

## Esimerkki

Kouramoottori ClawMotor pyörii asetettua nopeutta 25% asentoon 90 asetta.

```cpp
ClawMotor.setVelocity(25, percent);
ClawMotor.spinToPosition(90, degrees);
```

<advanced>
</advanced>