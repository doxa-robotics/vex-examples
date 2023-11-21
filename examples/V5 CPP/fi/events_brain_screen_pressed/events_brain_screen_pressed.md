category: events  
signature: Brain.Screen.pressed(callback);  
description: Runs the callback function when the V5 Brainâ€™s touchscreen is pressed.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

#  Aivojen näyttöä koskettu

Suorittaa ns callback -funktion, kun aivojen kosketusnäyttöä on kosketettu.

```cpp
Brain.Screen.pressed(callback);
```

## Miten käytetään

`Brain.Screen.pressed();`  komennon avulla voi laukaista toimintoja, kun näyttöä on koskettu. 

Yhdessä komennon `Brain.Screen.xPosition();` ja `Brain.Screen.yPosition();` kanssa saadaan interaktiivisuutta robotin ja käyttäjän välille.

Ensiksi pitää luoda funktio sille, kun näyttöä kosketaan ja sen nimi , jota käytetään callback-funktiossa parametrina , kun tapahtuma aktivoituu.

```cpp
//Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Event has occurred");
}

int main() {
  // Register event with a callback function.
  Brain.Screen.pressed(runOnEvent);

  while (true) {
    // Keep the main program running.
    wait(0.05, seconds);
  }
}
```


<advanced>
</advanced>