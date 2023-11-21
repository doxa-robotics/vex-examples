category: events  
signature: Brain.Screen.released(callback);  
description: Runs the callback function when the V5 Brainâ€™s touchscreen is released.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

#  Aivojen näyttöä vapautettu

Suorittaa ns callback funktion, kun aivojen kosketusnäyttöä on kosketus vapautetaan.

```cpp
Brain.Screen.released(callback);
```

## Miten käytetään

`Brain.Screen.released();` komennon avulla voi laukaista toimintoja näytön kosketuksen vapauttamisessa. 

Yhdessä komennon `Brain.Screen.xPosition();` ja `Brain.Screen.yPosition();` kanssa saadaan interaktiivisuutta robotin ja käyttäjän välille.

Ensiksi pitää luoda funktio sille, kun näyttöä kosketus loppuu ja nimi , jota käytetään callback-funtiossa parametrina , kun tapahtuma aktivoituu.

```cpp
//Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Event has occurred");
}

int main() {
  // Register event with a callback function.
  Brain.Screen.released(runOnEvent);

  while (true) {
    // Keep the main program running.
    wait(0.05, seconds);
  }
}
```


<advanced>
</advanced>