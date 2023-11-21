category: sensing  
signature: Drivetrain.temperature(percent)  
device_class: drivetrain  
description: Reports the temperature of the V5 Smart Motors powering the Drivetrain.

# Ajopelin moottorilämpötila

Antaa ajopelin ajomoottoreiden lämpötilan.

```cpp
Drivetrain.temperature(percent)
```

## Miten käytetään

`Drivetrain.temperature(percent)` antaa desimaaliarvon (muotoa *double*) , kun se raportoi ajopelin ajomoottoreiden lämpötilan.  

Komennot, jotka mittaavat arvoja voi laittaa muiden komentojen sisään kuten print komentoon tai toistorakenteissa ehtolausekkeisiin ilman puolipistettä.

Aseta `percent` yksiköksi ja arvot mitataan välillä **0.0% - 100.0%**. 

```cpp
Brain.Screen.print("%f", Drivetrain.temperature(percent));
```

<advanced>
</advanced>