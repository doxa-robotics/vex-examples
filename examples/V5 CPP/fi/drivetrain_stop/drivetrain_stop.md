category: drive  
signature: Drivetrain.stop();  
device_class: drivetrain  
description: Stops the Drivetrain.  

# Pysäytä

Pysäytä ajopeli.

`
```cpp
Drivetrain.stop();
```

## Miten käytetään

`Drivetrain.stop();` komento pysäyttää ajopelin. Sillä ei ole argumentteja.

## Esimerkki

Esimerkissä ajopeli pysähtyy kun se on ajanut 3 sekuntia eeenpäin.


```cpp
Drivetrain.drive(forward);
wait(3, seconds);
Drivetrain.stop();
```

<advanced>
</advanced>