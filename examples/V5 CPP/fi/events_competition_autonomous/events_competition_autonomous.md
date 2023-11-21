category: events  
signature: Competition.autonomous(callback);  
description: Runs the specified function when an "autonomous" mode signal is received from a competition field or competition switch.<br /><br />A competition object must be defined, or the program must be a competition template.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Kilpailu automaattikäynnistys

Suorittaa halutun funktion kun "automaatti" moodi signaali on kilpailuajon alussa saatu.

``cpp
Competition.autonomous(callback);
```

## Miten käytetään

Uusi kilpailu esiintymä voidaan luoda. kun  **driver_control** ja **automaatti** callback functiot on saatu.

Luo **automaatti** funktio, joka toimii kilpailutilanteessa. 

Tämä **automaatti** funktio suoritetaan kun "automaatti" moodi signaali on kilpailussa saatu.

varmista että kilpailuohjekti on määritelty tai käytä valmista mallia esimerkit ohjelmista.

``cpp
//Create a Competition Object
competition Competition;

//Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Event has occurred");
}

int main() {
  // Register event with a callback function.
  Competition.autonomous(runOnEvent);

  while (true) {
    // Keep the main program running.
    wait(0.05, seconds);
  }
}
```

<advanced>
</advanced>