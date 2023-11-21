category: motion  
signature: MOTOR393.setVelocity(50, percent);  
device_class: motor29
description: Sets the speed of a Motor393 connected to a Motor Controller 29. 

# Motor393 Aseta nopeus

Asettaa Motor393 nopeuden. Laite yhdistetty laitteeseen Motor Controller 29.

```cpp
Motor393.setVelocity(velocity, percent);
```

## Miten käytetään

Nopeus paramtri hyväksyy arvot välillä **-100% - 100%.** 

Jos asettaa Motor393 laitteeen nopeudeksi negatiivisen arvon, moottori pyörii taaksepäin.

TOheisessa esimerkissä moottori pyörii taaksepäin vaikka se on asetettu parametriarvoon`forward`.

```cpp
Motor393.set_velocity(-100, percent);
Motor393.spin(forward);
```

Jos asetaa nopeuden arvoksi 0, moottori pysähtyy.

<advanced>
</advanced>