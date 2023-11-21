category: drive  
signature: Drivetrain.setStopping(brake);  
device_class: drivetrain  
description: Sets the brake mode of the Drivetrain.  

# Aseta pysähtymistapa

Asettaa ajopelin pysähtymistavan.

```cpp
Drivetrain.setStopping(brakeType);
```

## Miten käytetään

Tässä pysähtymistavat `brakeType`parametrit, joita voi käyttää: 

* **brake** (jarruta) ajopeli pysähtyy heti , jos ulkopuolisia voimia ei esiinny
* **coast** (hitaasti) antaa ajopelin pysähtyä vaiheittain
* **hold** (lukitse) aiheuttaa ajopelin pysähtymisen ja asennon palautumisen pysähtymisasentoon , jos siihen vaikuttaa ulkoisia voimia

## Esimerkki

Esimerkissä ajopeli ajaa eteenpäin 3 sekuntia ja pysähtyy jarrujen lukituksella.

```cpp
Drivetrain.setStopping(hold);
Drivetrain.drive(forward);
wait(3, seconds);
Drivetrain.stop();
```

<advanced>
</advanced>