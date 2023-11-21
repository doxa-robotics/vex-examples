category: sensing  
signature: OPTICAL.isNearObject()  
device_class: optical  
description: Reports if a V5 Optical Sensor detects an object in its range  

# Optical on lähellä kohdetta/esinettä

Kertoo, havaitseeko V5 Optical Sensori näkökestässään kojdetta/esinettä.

```cpp
Optical.isNearObject()
```

## Miten käytetään

`Optical.isNearObject()` antaa arvon **true** jos esine on havaittu ja arvon **false** muuten.

IKomentoa kannattaa käyttää ja varmistaa arvo **true** aina ennen kuin käytetään `Optical.color()` komentoa itse värin etsimiseen.

```cpp
if (Optical.isNearObject() && Optical.color() == red) {
  Brain.Screen.print("Red object detected!");
}
```

<advanced>
</advanced>







