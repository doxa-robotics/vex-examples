category: events  
signature: BUMPER.pressed(callback);  
device_class: bumper  
description: Runs the specified function when the bumper is pressed.  

# Painokytkin painettu

Suorittaa tietyn **callback funktion** (taustafunktion) kun painokytkintä on painettu.

```cpp
Bumper.pressed(callback);
```

## Miten käytetään

Luodaan funktio, jota kutsutaan, kun Painokytkintä on painettu. Anna funktiolle nimi, joka suoritetaan kun tapahtuma sattuu `callback` parametrissa.

```cpp
void bumperPressed() {
  Brain.Screen.print("Bumper pressed.");
}
```
Funktion nimi välitetään `Bumper.pressed` funktiokutsun parametrina.

```cpp
Bumper.pressed(bumperPressed);
```

## Callback Functions (Taustafunktiot)

Callback funktio on funktio, joka välitetään toiselle funktiolle argumenttina. **Callback funktion** koodi suoritetaan kun tapahtuma **event** sattuu. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  Bumper.pressed(callbackFunction);
}
```

<advanced>
</advanced>