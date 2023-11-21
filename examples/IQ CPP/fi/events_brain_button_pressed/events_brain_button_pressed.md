category: events  
signature: Brain.buttonUp.pressed(callback);  
description: Runs the callback function when the Brainâ€™s touchscreen is pressed.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

#  Aivojen painiketta painettu

Suorittaa ns callback funktion kun VEX IQ Aivojen nappia on painettu.

```cpp
Brain.Button.pressed(callback);
```

## Miten käytetään

Pitää luoda funktio , jota kutsutaan, kun Aivojen nappia on painettu.

```cpp
void buttonPressed() {
  Brain.Screen.print("Button pressed.");
}
```

`Brain.Button.pressed` funktion voi kohdistaa VEX IQ Aivojen nappeihin.

- `Brain.buttonUp.pressed(buttonPressed);` Ylös-nappi
- `Brain.buttonDown.pressed(buttonPressed);`Alas -nappi
- `Brain.buttonCheck.pressed(buttonPressed);`Check-nappi

## Callback funktiot

Callback -funktio on funktio, joka välitetään toiselle funktiolle argumenttina. **Callback funktion** koodi suoritetaan kun ko tapahtuma **event** sattuu. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  Brain.Button.pressed(callbackFunction);
}
```

<advanced>
</advanced>