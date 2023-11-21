category: sensing  
signature: VISION.objects[0].exists;  
device_class: vision  
description: Reports if the Vision Sensor detects a configured object. 

# Kohde löytyy

Raportoi jos Vision -kamera näkee kuvassa sille määritellyn kohteeen. 

Kohde pitää aina määritellä ennen kuin `Vision.objects[index].exists` komentoa voi käyttää etsimään kohdetta.

```cpp
Vision.objects[index].exists
```

## Miten käytetään

Tee tarkemmat kohteen määrityksen enne kuin voit käyttää tätä komentoa. 


`Vision.objects[index].exists` antaa arvon **tosi** kun Vision -kamera havaitsee kohteen merkin/värikoodin.

`Vision.objects[index].exists` antaa arvon **epätosi** kun Vision -kamera ei havaitse kohteen merkiä/värikoodia.

Aina enne analysointia pitää ottaa kuva ts suorittaa `Vision.takeSnapshot()` -komento.


```cpp
if(Vision.objects[0].exists){

}
```

<advanced>
</advanced>