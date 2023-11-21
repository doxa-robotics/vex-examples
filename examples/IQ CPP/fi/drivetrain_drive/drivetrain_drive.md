category: drive  
signature: Drivetrain.drive(forward);  
device_class: drivetrain  
description: Moves the Drivetrain forever. All drivetrain motors are run forwards or backwards at the speed that was set using `Drivetrain.setDriveVelocity`, the default speed is 50 rpm.

# Aja

Ajopeli liikkuu jatkuvasti (ikuisesti).

```cpp
Drivetrain.drive(direction);
```

Kaikki ajopelin ajomoottorit pyörivät eteen- tai taaksepäin nopeuden `Drivetrain.setDriveVelocity`-kommennon mukaisesti. Oletuksena on ilman asetusta 50 kierrosta minuutissa.

## Miten käytetään

`Drivetrain.drive` komennolla ajopeli liikkuu ikuisesti kunnes uusi ajopelikomento on asetettu tai ohjelma päättyy.

Valitse **forward** (eteenpäin) parametri ,jos haluat ajopelin ajavan eteenpäin.

```cpp
Drivetrain.drive(forward);
```

Valitse **reverse** (taaksepäin) parametri ,jos haluat ajopelin ajavan (peruuttavan) taaksepäin .

```cpp
Drivetrain.drive(reverse);
```
 
<advanced>
</advanced>