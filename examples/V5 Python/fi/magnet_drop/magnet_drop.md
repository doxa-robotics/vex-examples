category: magnet  
signature: magnet.drop() 
description: Allows the V5 Electromagnet to drop the object it is currently holding.  


# Sähkömagneetti pudottaa

Antaa sähömagneetille käskyn pudottaa siinä oleva esine.

```
magnet.drop()
```
Kun komento `magnet.drop()` on suoritettu, pitää magneetin jäähtyä ennen uutta käyttöä.

## Esimerkki

Poimitaan esine , ajetaan robottia eteenpäin ja käytetään `magnet.drop()` komentoa esineen pudotukseen.

```
magnet.pickup()
drivetrain.drive_for(FORWARD, 200, MM)
magnet.drop()
```

<advanced>
</advanced>