category: drive  
signature: Drivetrain.turnFor(right, 90, degrees);  
device_class: drivetrain  
description: Turns the Drivetrain for a distance.  

# Käänny määrä

Kääntää ajopeliä määrätyn määrän asteita.


```cpp
Drivetrain.turnFor(turnType, angle, units);
```

## Miten käytetään

Ensimmäinen argumentti komennossa määrää suunnan: `LEFT` (vasemmalle) tai `RIGHT` (oikelle), isoilla kirjaimilla . 

Toinen argumentti määrää kulman asteina välillä  0 - 360. 

Kolmas argumentti on käännöksen yksikkö, Se on `DEGREES` (astetta) isoilla kirjaimilla. 

Komento`turn_for` on ns blokkaava komento ts se estää seuraavien komentojen suorituksen , kunnes käännös on valmis.

## Lisäparametrit

Neljäs argumetti on ns lisäargumentti `wait=False` , jolloin seuraava komento suoritetaankin heti käännöksen alettua.


```cpp
Drivetrain.turnFor(left, 90, degrees, false);
```


## Esimerkki

Esimerkissä V5 Robotti kääntyy 270 astetta oikealle.

````cpp
Drivetrain.turnFor(right, 270, degrees);
```


<advanced>
</advanced>
