category: drive  
signature: Drivetrain.setStopping(brake);  
device_class: drivetrain  
description: Sets the brake mode of the Drivetrain.  

# Pysäytä ajo


```cpp
Drivetrain.setStopping(brakeType);
```

## Miten käytetään

Aseta `brakeType` parametrille joku seuraavista valinta:

* brake: pysäytttää ajopelin heti.
* coast: ajopeli pysähtyy vähittellen.
* hold: pysäyttää ajopelin heti ja pitää pysähdysasennon, vaikka ajopeli liikkuisi muuten esim esineen päältä liukuen alas. 

 `drivetrain.set_stopping()` komento pysyy voimassa jatkossakin niin kauan kunnes tehdään uusi määritys pysähdystavalle.
 
## Esimerki

Esimerkissä ajopeli ajaa eteenpäin 3 sekuntia ennen kuin pysähtyy paikalleen.

```cpp
Drivetrain.setStopping(hold);
Drivetrain.drive(forward);
wait(3, seconds);
Drivetrain.stop();
```


<advanced>
</advanced>