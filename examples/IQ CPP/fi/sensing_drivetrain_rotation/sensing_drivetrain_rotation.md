category: sensing  
signature: Drivetrain.rotation(degrees)  
device-class: drivetrain
description: Reports the Drivetrain's angle of rotation in degrees when configured with a VEX IQ Gyro Sensor.

# Ajopelin Käännös asteina

Raportoi ajopelin kääntymiskulman asteina

```cpp
Drivetrain.rotation(degrees)
```

## Miten käytetään

`Drivetrain.rotation` raportoi kasvavan kulman arvon, jos ajopeli kääntyy **vastapäivään**.

`Drivetrain.rotation` raportoi pienenevän kulman arvon, jos ajopeli kääntyy **myötäpäivään**.

## Esimerkki

Esimerkissä tulostetaan ajopelin kääntymiskulma VEX IQ Aivojen näytölle.

```cpp
Drivetrain.turn(left);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Drivetrain Rotation: %.2f", Drivetrain.rotation(degrees));

  // Pieni odotus ettei tulostu sotkua
  wait(20, msec);
}
```

<advanced>
</advanced>