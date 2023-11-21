category: events  
signature: Controller.Button.pressed();  
description: Runs the callback function when the Controller button is pressed.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.

# Ohjaimen nappia painettu

Suorittaa ns **callback funktion**, kun VEX IQ Ohjaimen tiettyä nappia on painettu.

```cpp
Controller.Button.pressed(callback);
```

## Miten käytetään

Luodaan oma **Callback funktio**, jota kutsutaan nimettynä parametrina tapahtumassa, kun Ohjaimen tiettyä painonappia on painettu.

```cpp
void buttonPressed() {
  Brain.Screen.print("Button pressed.");
}
```

Valitse mitä nappia käytetään painettu `pressed()` funktiossa.

![controller_button_back](controller_button_front.jpg)

- `Controller.ButtonEUp.pressed(buttonPressed);` EYlä
- `Controller.ButtonEDown.pressed(buttonPressed);` EAla
- `Controller.ButtonFUp.pressed(buttonPressed);` FYlä
- `Controller.ButtonFDown.pressed(buttonPressed);` FAla

![controller_button_front](controller_button_back.png)

- `Controller.ButtonLUp.pressed(buttonPressed);` LYlä
- `Controller.ButtonLDown.pressed(buttonPressed);` LAla
- `Controller.ButtonRUp.pressed(buttonPressed);` RYlä
- `Controller.ButtonRDown.pressed(buttonPressed);` RAla

<advanced>
</advanced>