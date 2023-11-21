category: sensing  
signature: Brain.Button.pressing()  
description: Reports if a button on the VEX IQ Brain is pressed.

# Aivojen painiketta painettu

Raportoi jos tiettyä VEX IQ aivojen painiketta on painettu.

```cpp
Brain.Button.pressing()
```

## Miten käytetään

Raportoi arvon **tosi** jos tiettyä Aivojen painiketta on painettu ja arvon **epätosi** jos painiketta ei ole painettu.

`Brain.` jälkeen pitää antaa painike, jota tarkastelaan. 

Tuetut painikkeet ovat:
- `Ylös`
- `Alas`
- `Tarkista`

## Esimerkki

Esimerkissä VEX IQ robotti ajaa eteenpäin.

Kun aivojen **Alas** painiketta painetaan se kääntyy heti oikealle.

```cpp
Drivetrain.drive(forward);

while (true) {
  if (Brain.buttonUp.pressing()) {
    Drivetrain.turn(right);
    break;
  }

  wait(20, msec);
}
```

<advanced>
</advanced>