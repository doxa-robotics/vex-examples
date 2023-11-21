category: drive  
signature: Drivetrain.setTimeout(1, seconds);  
device_class: drivetrain  
description: Sets the timeout for the Drivetrain to stop moving if a blocking command cannot reach its target.  

# Aseta aikaraja

`Drivetrain.setTimeout();` asettaa aikarajan, kuinka kauan robotin liikekomento jatkuu.

``cpp
Drivetrain.setTimeout(time, seconds);
```

## Miten käytetään

Komentoa käytetään estämään ohjelman keskeytys, jos seuraava liikekomento ei pääse tavoiteasemaan esimerkiksi kun robotti törm'' laitaan tai muuhun esteeseen

Aseta määrä sekunteina `SECONDS`.


```cpp
Drivetrain.setTimeout(2.0, seconds);
```
## Esimerkki

Esimerkissä on asetettu 3 sekunnin aikaraja ajo komennolle.

```cpp
Drivetrain.setTimeout(2.0, seconds);
Drivetrain.driveFor(24.0, inches, true);
Drivetrain.turnFor(90.0, degrees, true);
```



<advanced>
</advanced>