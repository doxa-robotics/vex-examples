category: sensing  
signature: Gyro.rotation()  
device_class: gyro  
description: Reports the Gyro Sensor's current rotation in degrees.

# Gyron kiertokulma asteina

Antaa VEX IQ Gyro Sensorin mnykyisen asennon asteina.

```cpp
Gyro.rotation()
```

## Miten käytetään

`Gyro.rotation` raportoi kasvavia arvoja kun Gyro Sensori kääntyy **counter-clockwise** vastapäivään.

`Gyro.rotation` raportoi pieneneviä arvoja kun Gyro Sensori kääntyy **clockwise** myötäpäivään.

## Esimerkki

Esimerkissä tulostetaan Gyro Sensorin arvo VEX IQ Aivojen näytölle.

```cpp
Drivetrain.turn(left);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Gyro Rotation: %.2f", Gyro.rotation());

  // Odotus ettei tule päällekkäistulostusta tai sotkua
  wait(20, msec);
}
```

<advanced>
</advanced>