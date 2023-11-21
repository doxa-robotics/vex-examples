category: motion  
signature: MOTOR393.stop();  
device_class: motor29
description: Stops a Motor393 connected to a Motor Controller 29.

# Motor393 Pysäytä

Pysäyttää Motor393 , joka on liitetty Motor Controller 29 laitteeseen.

```cpp
Motor393.stop();
```

## Miten käytetään

Komento pysäyttää Motor393 laitteen pyörimisen.

## Esimerkki

Motor393 pyörii 3 sekuntia ennen kuin se pysähtyy.

```cpp
Motor393.spin(forward);
wait(3, seconds);
Motor393.stop();
```

<advanced>
</advanced>