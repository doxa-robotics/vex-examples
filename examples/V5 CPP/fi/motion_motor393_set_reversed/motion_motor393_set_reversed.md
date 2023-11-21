category: motion  
signature: MOTOR393.setReversed(true);  
device_class: motor29
description: Reverses the spin direction of a Motor 393 connected to a Motor Controller 29.

# Motor393.setReversed();

Muttaa pyörimissuunnan vastakkaiseen moottorissa Motor 393 , joka kiinnitetty Motor Controller 29 laitteeseen.

```cpp
Motor393.setReversed();
```

## Miten käytetään

Komennolla moottori pyörii vastakkaiseen suuntaan.

`Motor393.setReversed();` hyväksyy Boolean argumentit `true` ja `false`.

## Esimerkki

Seuraavassa esimerkissä moottori pyörii taaksepäin `Motor393.setReversed();` komennon mukaan.

```cpp
Motor393.setReversed(true);
Motor393.spin(forward);
```

<advanced>
</advanced>