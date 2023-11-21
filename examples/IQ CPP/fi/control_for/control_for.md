category: control  
signature: control_for
description: A type of loop that repeats the code contained inside for a set number of iterations. 

# Toista

Toistetaan aaltosulkujen sisällä oleva koodi halutun kertamäärän.

```cpp
for (initialization; condition; increment/decrement) {
  // koodi, jota toistetaan
}
```

## Miten käytetään

Anna lukumäärä, joka toistetaan ehdossa **repeat** käyttäen kolmea parametria:

* initialization (alkuarvo)
* condition (ehto)
* increment/decrement (askel)

**Initialization** asetaa alkuarvon toistomuuttujalle.

**Condition** asettaa ehdon, kuinka kauan koodia toistetaan. Toistetaan kunnes toistoehto toteutuu eli se saa arvon tosi **false**.

**Increment/decrement** vaihtaa iterointimuuttujan askelarvoa loopin lopussa laskukaavalla.

## Esimerkki 1

Esimerkissä tulostetaan luvut välillä  0 arvoon 9 VEX IQ aivojen näytölle.

```cpp
for (int i = 0; i < 10; i++) {
  Brain.Screen.print("%d", i);
  wait(20, msec);
}
```
## Esimerkki 2

esimerkissä ajopeli ajaa ensin eteenpäin 10 tuumaa ja sitten kääntyy 60 astetta oikealle kolme kertaa peräkkäin. 

```cpp
Drivetrain.driveFor(forward, 10.0, inches);

for (int i = 0; i < 3; i++) {
  Drivetrain.turnFor(right, 60, degrees);
  wait(20, msec);
}
```

<advanced>
</advanced>