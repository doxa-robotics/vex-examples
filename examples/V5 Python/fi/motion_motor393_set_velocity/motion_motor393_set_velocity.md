category: motion  
signature: motor393.set_velocity(10, PERCENT)  
description: Sets the speed of a Motor393.

# Aseta Moottori Controller Nopeus

Asettaa Motor393 nopeuden yhdistettynä moottori Controller 29.

```python
motor393.set_velocity(VELOCITY, PERCENT)
```

## Miten käytetään

`VELOCITY` parametriin voi asettaa arvot välillä -100% - 100%.

Asettamalla negatiivisen arvon moottori pyörii taaksepäin.

Alla olevassa esimerkissä moottori pyörii taaksepäin vaikka `FORWARD` parametri on käytössä.

```python
motor393.set_velocity(-100, PERCENT)
motor393.spin(FORWARD)
```

Jos asettaa Motor393nopeuden arvoon 0 moottori pysähtyy.

<advanced>
</advanced>
