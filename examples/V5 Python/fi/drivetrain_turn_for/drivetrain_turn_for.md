category: drive  
signature: drivetrain.turn_for(RIGHT, 90, DEGREES, wait=True) 
description: Turns the Drivetrain for a given distance.  

# Käänny määrä

Kääntää ajopeliä määrätyn määrän asteita.

```don
drivetrain.turn_for(DIRECTION, ANGLE, UNITS)
```

## Miten käytetään

Ensimmäinen argumentti komennossa määrää suunnan: `LEFT` (vasemmalle) tai `RIGHT` (oikelle), isoilla kirjaimilla . 

Toinen argumentti määrää kulman asteina välillä  0 - 360. 

Kolmas argumentti on käännöksen yksikkö, Se on `DEGREES` (astetta) isoilla kirjaimilla. 

Komento`turn_for` on ns blokkaava komento ts se estää seuraavien komentojen suorituksen , kunnes käännös on valmis.

## Lisäparametrit

Neljäs argumetti on ns lisäargumentti `wait=False` , jolloin seuraava komento suoritetaankin heti käännöksen alettua.

```don
drivetrain.turn_for(LEFT, 90, DEGREES, wait=False)
```

## Esimerkki

Esimerkissä V5 Robotti kääntyy 270 astetta oikealle.

```don
drivetrain.turn_for(RIGHT, 270, DEGREES)
```

<advanced>
</advanced>
