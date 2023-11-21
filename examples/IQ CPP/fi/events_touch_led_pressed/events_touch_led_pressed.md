category: events  
signature: TouchLED.pressed(callback);  
device_class: TouchLED  
description: Runs the specified callback function when the Touch LED is pressed.  

# KosketusLED painettu

Suorittaa määrätyn **callback funktion** kun KosketusLED painiketta on painettu.

```cpp
TouchLED.pressed(callback);
```

## Miten käytetään

Luodaan funktio, jota kutsutaan, kun KosketusLED painettu. Nimeä funktio, joka suoritetaan, kun haluttu tapahtuma 'event' sattuu ja anna se  `callback` parametrina.

```cpp
void touchLEDPressed() {
  Brain.Screen.print("Touch LED pressed.");
}
```
Then, the function is passed as the parameter of the `TouchLED.pressed` function call.

```cpp
TouchLED.pressed(touchLEDPressed);
```

## Callback Funktiot

Callback funktio on funktio, joka välitetään toiseen funktioon argumenttina. **Callback function** komennot suoritetaan kun **event** eli tapahtuma sattuu. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  TouchLED.pressed(callbackFunction);
}
```

<advanced>
</advanced>