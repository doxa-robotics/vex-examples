category: sensing  
signature: Drivetrain.torque(Nm)  
device_class: drivetrain  
description: Reports the amount of torque (rotational force) the Drivetrain is currently using.

# Ajopelin ajomoottoreiden vääntövoima

Antaa vääntövoiman (kiertovoiman), jota ajopelin moottorit tällä hetkellä tuottaa.

```cpp
Drivetrain.torque(Nm)
```

## Miten käytetään

`Drivetrain.torque(Nm)` antaa arvona desimaaliluvun (muotoa *double*), kun se raportoi ajopelin ajomoottoreiden vääntövoiman. 

Oletuksena on yksikkö Newton-meters(`Nm`), jolla mitattuna arvot vaihtelee välillä **0.0 - 2.1 Newton-metriä (Nm)**.

Vaihtoehtona on yksikkö Tuuma Pauna (`InLB`).

```cpp
Brain.Screen.print("%f", Drivetrain.torque(Nm));
Brain.Screen.print("%f", Drivetrain.torque(InLb));
```
<advanced>
</advanced>