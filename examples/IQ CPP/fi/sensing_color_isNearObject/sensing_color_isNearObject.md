category: sensing  
signature: Color.isNearObject()  
description: Reports if the Color Sensor is near an object.

# Värisensori Havaitsee värin?

Raportoi näkeekö Värisensori esineen tai pinnan värin. 

```cpp
Color.isNearObject()
```

## Miten käytetään

Ensimmäinen osa komentoa on nimetty värisensori.

```cpp
Color5.isNearObject()
Color7.isNearObject()
```

Antaa arvon **tosi**, jos värisensori havaitsee esineen tai pinnan värin edessään. 

Antaa arvon **epätosi**, jos värisensori ei havaitse esineen tai pinnan väriä edessään. 

## Esimerkki

Tulostetaan Aivojen näytölle, näkeekö nimetty värisensori väriesineen edessään.

```cpp
Brain.Screen.print("Is Near Object: %s", Color.isNearObject() ? "TRUE" : "FALSE");
```

<advanced>
</advanced>