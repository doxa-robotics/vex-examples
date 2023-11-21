category: events  
signature: TouchLED.released(callback);  
device_class: touchled  
description: Runs the specified callback function when the Touch LED is released.  

# KosketusLED vapautettu

Suorittaa määrätyn **callback funktion**, kun KosketusLED on vapautettu.

```cpp
TouchLED.released(callback);
```

## Miten käytetään

Sinun pitää luoda nimetty kutsufunktio esim touchLEDReleased, joka suoritetaan kun ko tapahtuma sattuu

```cpp
void touchLEDReleased() {
  Brain.Screen.print("Touch LED released.");
}
```
Funktion nimi välitetään parametrina valmiin `TouchLED.released` funktion kutsuparametrissa.

```cpp
TouchLED.released(touchLEDReleased);
```

## Callback Funktiot

callback funktio on funktio, jonka nimi välitetään argumenttina  **callback funktion** sisällä, kun tapahtuma **event** sattuu. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  TouchLED.released(callbackFunction);
}
```

<advanced>
</advanced>