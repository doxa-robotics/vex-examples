category: drive  
signature: Drivetrain.drive(forward);  
device_class: drivetrain  
description: Moves the Drivetrain forever. All drivetrain motors are run forwards or backwards at the speed that was set using `Drivetrain.setDriveVelocity`, the default speed is 50 rpm.

# Aja

Ajopeli liikkuu ikuisuuden suuntaan, joka määritelty suluissa. 

Kaikki ajopelin ajomoottorit ajavat eteen tai taaksepäin nopeutta , joka on määritelty komennolla `Drivetrain.setDriveVelocity`, oletus on 50%. 

Negatiiviset nopeusarvot aiheuttavat sen, etttä ajopeli ajaa vastakkaiseen suuntaan parametrilla  FORWARD .

```cpp
Drivetrain.drive(directionType);
```

## Miten käytetään

`Drivetrain.drive();` komennolla ajopeli ajaa ikuisuuden kunnes joku uusi ajokomento on annettu tai ohjelma on lopetettu.

## Esimerkit

Käytä `forward` argumenttia , kun ajopeli ajaa eteenpäin

```cpp
Drivetrain.drive(forward);
```

Käytä `reverse` argumenttia , kun ajopeli peruuttaa.

```cpp
Drivetrain.drive(reverse);
```
 
<advanced>
</advanced>