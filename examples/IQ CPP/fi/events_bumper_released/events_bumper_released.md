category: events  
signature: Bumper.released(callback);  
device_class: bumper  
description: Runs the specified function when the bumper is released.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Painokytkin vapautettu

Suorittaa tietyn funktion kunn painaokytkin on vapautettu.

```cpp
Bumper.released(callback);
```

## Miten käytetään

Luiodaan funktio, jota kutsutaan kun Painokytkin on vapautettu. Anna funktiolle nimi joka annetaan `callback` (kutsu) parametrina.

```cpp
void bumperReleased() {
  Brain.Screen.print("Bumper released.");
}
```
Nimetty funktio välitetään `Bumper.released` funktion kutsussa parametrina.

```cpp
Bumper.released(bumperReleased);
```

## Callback Funktiot

callback funktion on funktio, joka välitetään toiselle funktiolle parametrina . **callback function** suoritetaan kun ko tapahtuma **event** tapahtuu. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Callback Function Called.");
}

int main() {
  Bumper.released(callbackFunction);
}
```

<advanced>
</advanced>