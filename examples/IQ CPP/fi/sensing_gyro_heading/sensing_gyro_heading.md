category: sensing  
signature: Gyro.heading() 
device_class: gyro  
description: Reports the Gyro Sensor's current heading in degrees.

# Gyro Ajosuunta

Raportoi Gyro Sensorin nykyisen ajosuunnan asteina.

```cpp
Gyro.heading()
```

## Miten käytetään

`Gyro.heading` komento antaa kasvavia arvoja kun käännytään **vastapäivään**.

`Gyro.heading` antaa arvoja välillä **0.00 to 359.99**.

## Esimerkki

Esimerkissä tulostetaan Gyro Sensorin ajosuunta VEX IQ aivojen näytölle.

```cpp
Drivetrain.turn(left);

while (true) {
  Brain.Screen.clearScreen();
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Gyro Heading: %.2f", Gyro.heading());

  // Brief delay to prevent print distortion or tearing
  wait(20, msec);
}
```

<advanced>
</advanced>