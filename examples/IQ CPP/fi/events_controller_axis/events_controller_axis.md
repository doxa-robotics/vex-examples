category: Events
signature: `Controller.AxisA.changed(callback)`  
device_class: Controller
description: Runs callback funtion when the selected VEX IQ Controller joystick axis is moved.

# Ohjaimen tattia käännetty

Suorittaa tietyn callback funktion, kun VEX IQ ohjaimen joystick tattia on liikutettu.

```cpp
Controller.Axis.changed(callback);
```

## Miten käytetään

Luodaan oma ns callback funktio, jota kutsutaan kun ohjaintattia on liikutettu.

```cpp
void axisMoved() {
  Brain.Screen.print("Axis moved.");
}
```

valise mätä ohjaintattia käytetään funktiossa

- `Controller.AxisA.changed(axisMoved);` A-tappi
- `Controller.AxisB.changed(axisMoved);` B-tatti
- `Controller.AxisC.changed(axisMoved);` C-tatti
- `Controller.AxisD.changed(axisMoved);` D-tappi

![controller_button_front](controller_button_front.jpg)

## Callback funktiot

Callback funktio on funktionimi, joka välitetään toiselle funktiolle argumenttina. **Callback funktion** koodi suoritetaan kun ko tapahtuma **event** sattuu. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  Controller.AxisA.changed(callbackFunction);
}
```

<advanced>
</advanced>