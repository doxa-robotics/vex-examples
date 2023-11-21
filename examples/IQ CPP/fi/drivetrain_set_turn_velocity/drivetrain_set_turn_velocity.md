category: drivetrain
signature: Drivetrain.setTurnVelocity(50, percent);  
device_class: drivetrain  
description: Sets the velocity of the Drivetrain when turning. If this is used when the drivetrain is turning, the drivetrain will be updated with the new speed.  

# Aseta kääntymisnopeus

Asettaa ajopelin kääntymisnopeuden. 

Jos asetus tehdään kesken kääntymisen nopeus päivitetään ajon aikana.

```cpp
Drivetrain.setTurnVelocity(velocity, units);
```

## Miten käytetään

`Drivetrain.setTurnVelocity` asettaa vain kääntyminopeuden ts se ei liiikuta ajopeliä. 

`Drivetrain.setTurnVelocity` hyväksyy arvot välillä **-100 - 100** kun yksikkönä on **percent** (prosenttia).

`Drivetrain.setTurnVelocity` hyväksyy arvot välillä **-127 - 127** kun yksikkönä on **rpm** (kierrosta minuutissa).

Asettanmalla ajopelin kääntymisnopeudeksi negatiivisen arvon, ajopeli kääntyy vastakkaiseen suuntaan.

Jos kääntymiselle asettaa arvon 0 , se estää kääntymisen.

## Esimerkki

Esimerkissä ajopeli kääntyy vasemmalle nopeudella 25% prosenttia.

```cpp
Drivetrain.setTurnVelocity(25, percent);
Drivetrain.turn(left);
```

<advanced>
</advanced>
