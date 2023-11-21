category: events  
signature: Brain.button.released();  
description: Runs the callback function when the Brainâ€™s touchscreen is released.  

# Aivojen painike vapautettu

Suorittaa ns callback funktion, kun tiettyä VEX IQ Aivojen painike on vapautettu.

```cpp
Brain.Button.released(callback);
```

## Miten käytetään

Pitää luoda funktio, joka kutsutaan, kun tietty Aivojen painike vapautettavan.

```cpp
void buttonReleased() {
  Brain.Screen.print("Button released.");
}
```

`Brain.Button.released` funktiota voi käyttää eri VEX IQ Aivojen painikkeisiin.

- `Brain.buttonUp.released(buttonReleased);` Ylös
- `Brain.buttonDown.released(buttonReleased);` Alas
- `Brain.buttonCheck.released(buttonReleased);`Check

## Callback Funktiot

Callback funktio on funktio, joka asetataan toisen funktion argumentiksi. **Callback funktion** koodi suoritetaan kun tapahtuma **event** sattuu. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  Brain.Button.released(callbackFunction);
}
```

<advanced>
</advanced>