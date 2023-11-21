category: sensing  
signature: ENCODER.position(degrees)  
device_class: encoder  
description: Reports the distance the Shaft Encoder has rotated.

# Kierrosmittarin asento

Antaa akselin kierrosmittarin pyörimän matkan.

```cpp
Encoder.position(units)
```

## Miten käytetään

`Encoder.position()` palauttaa desimaaliluvun muotoa (*double*) , kun se antaa kierrosmittarin mittaaman matkan.


Tällaisia komentioja voi käyttää arvoina muissa komennoissa mm tulostuksessa tai ohjauslausekkeissa osana ehtoja.


Yksikkönä voi olla asteita `degrees` .

```cpp
Brain.Screen.print("%f", EncoderC.position(degrees));
```

Yksikkönä voi olla akselin kierroksia  `turns`.

```cpp
Brain.Screen.print("%f", EncoderC.position(turns));
```
<advanced>
</advanced>