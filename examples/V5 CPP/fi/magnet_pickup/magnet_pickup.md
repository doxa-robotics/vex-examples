category: magnet  
signature: MAGNET.pickup();  
device_class: electromagnet  
description: Energize a V5 Electromagnet to pick up a magnetic object  

# Sähkömagneetin avulla poiminta

Antaa käskyn V5 sähkömagneetille poimia esine.

```
Magnet.pickup();
```
Komennon `magnet.pickup()` jälkeen pitää magneetin jäähtyä ennen seuraavaa magneettikomentoa.

## Esimerkki

Esimerkissä `magnet.pickup()` poimii esineen , ajopeli aja eteenpäin ja pudottaa esineen.

```cpp
Magnet.pickup();
Drivetrain.driveFor(forward, 200, mm);
Magnet.drop();
```

<advanced>
</advanced>






