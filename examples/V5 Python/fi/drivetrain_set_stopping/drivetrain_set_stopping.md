category: drivetrain
signature: drivetrain.set_stopping(BRAKE)
description: Sets the behavior of the V5 robot's Drivetrain once it stops moving.  
# Pysäytä ajo

```python
drivetrain.set_stopping(MODE)
```

## Miten käytetään

Aseta `MODE` parametrille joku seuraavista valinta:

* BRAKE: pysäytttää ajopelin heti.
* COAST: ajopeli pysähtyy vähittellen.
* HOLD: pysäyttää ajopelin heti ja pitää pysähdysasennon, vaikka ajopeli liikkuisi muuten esim esineen päältä liukuen alas. 

 `drivetrain.set_stopping()` komento pysyy voimassa jatkossakin niin kauan kunnes tehdään uusi määritys pysähdystavalle.
 
## Esimerki

Esimerkissä ajopeli ajaa 200 mm ennenkuin se pysähtyy vähitellen -optiolla.


```python
drivetrain.set_stopping(COAST)
drivetrain.drive_for(FORWARD, 200, MM)
```
<advanced>
</advanced>
