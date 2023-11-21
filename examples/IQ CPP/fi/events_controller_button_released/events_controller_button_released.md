category: events  
signature: Controller.Button.released();  
description: Runs the callback function when the Controller button is released.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.

# Ohjaimen nappi vapautettu

Suorittaa **callback funktion** kun VEX IQ Ohjainen nappi on vapautettu.

```cpp
Controller.Button.released(callback);
```

## Miten käytetään

Pitää luoda ns **callback funktio** ,jota kutsutaan kun Ohjaimen tietty nappi on vapautettu.

```cpp
void buttonReleased() {
  Brain.Screen.print("Button released.");
}
```

Valise minkä napin otat käyttöön, kun kutsut `released()` funktiota.

- `Controller.ButtonEUp.released(buttonReleased);`
- `Controller.ButtonEDown.released(buttonReleased);`
- `Controller.ButtonFUp.released(buttonReleased);`
- `Controller.ButtonFDown.released(buttonReleased);`
- `Controller.ButtonLUp.released(buttonReleased);`
- `Controller.ButtonLDown.released(buttonReleased);`
- `Controller.ButtonRUp.released(buttonReleased);`
- `Controller.ButtonRDown.released(buttonReleased);`

![controller_button_back](controller_button_front.jpg)


![controller_button_front](controller_button_back.png)

## Callback Funktiot

Callback -funktio on funktio joka viedään toisen funktion argumentiksi. **Callback funktio** suoritetaan kun tapahtuma eli **event** sattuu. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  Controller.ButtonRDown.released(callbackFunction);
}
```

<advanced>
</advanced>