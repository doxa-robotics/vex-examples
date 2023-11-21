category: sensing  
signature: BUMPER.pressing()  
device_class: bumper  
description: Reports if the Bumper Switch is pressed.

# Painokytkintä on painetttu
 
Antaa tiedon, onko painokytkintä painettu.

```cpp
Bumper.pressing()
```

## Miten käytetään

bumper.pressing() antaa arvon **True** (tosi), jos painokytkintä on painettu.

bumper.pressing() antaa arvon **False** (epätosi), jos painokytkintä ei ole painettu.

```cpp
waitUntil(BumperA.pressing());
Brain.Screen.print("BumperA pressed!");
```
<advanced>
</advanced>