category: sensing  
signature: DISTANCE.objectSize()  
device_class: distance  
description: Reports an estimation of the detected object's size  

# Havaitun esineen koko

Anta arvion esineen koosta , jonka tisyysanturi havaitsee.

```cpp
Distance.objectSize()
```

## Miten käytetään

`Distance.objectSize()` avulla voidaan arvioida havaitun esineen kokoa.

Kokoja on kolme:

* sizeType::large (iso)
* sizeType::medium (keskikoko)
* sizeType::small (pieni)

```cpp
if (Distance.objectSize() == sizeType::large) {
  Brain.Screen.print("Large object detected!");
}
```

<advanced>
</advanced>





