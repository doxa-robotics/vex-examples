category: magnet  
signature: magnet.pickup() 
description: Allows the V5 Electromagnet to pickup an object.

# Sähkömagneetin avulla poiminta

Antaa käskyn V5 sähkömagneetille poimia esine.

```
magnet.pickup()
```
Komennon `magnet.pickup()` jälkeen pitää magneetin jäähtyä ennen seuraavaa magneettikomentoa.

## Esimerkki

Esimerkissä `magnet.pickup()` poimii esineen , ajopeli aja eteenpäin ja pudottaa esineen.

```
magnet.pickup()
drivetrain.drive_for(FORWARD, 200, MM)
magnet.drop()
```

<advanced>
</advanced>