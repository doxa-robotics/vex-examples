category: magnet  
signature: MAGNET.drop();  
device_class: electromagnet  
description: Energize a V5 Electromagnet to drop an attached object  

# Sähkömagneetti pudottaa

Antaa sähömagneetille käskyn pudottaa siinä oleva esine.

```
Magnet.drop()
```
Kun komento `magnet.drop()` on suoritettu, pitää magneetin jäähtyä ennen uutta käyttöä.

## Miten käytetään esimerkki

Poimitaan esine , ajetaan robottia eteenpäin ja käytetään `magnet.drop()` komentoa esineen pudotukseen.

```cpp
Magnet.pickup();
Drivetrain.driveFor(forward, 200, mm);
Magnet.drop();
```

<advanced>
</advanced>





