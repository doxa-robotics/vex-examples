category: events  
signature: Competition.drivercontrol(callback);  
description: Runs the specified function when an "driver control" mode signal is received from a competition field or competition switch.<br /><br />A competition object must be defined, or the program must be a competition template.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Kilpailu ohjainkäynnistys

Suorittaa halutun funktion kun "ohjainajo" moodi signaali on kilpailuajon alussa saatu.

```cpp
Competition.drivercontrol(callback);
```


## Miten käytetään

Uusi kilpailu esiintymä voidaan luoda kun  **ohjainajo** ja **automaatti** callback -funktiot on saatu.

Luo **ohjainkäynnistys** funktio, joka toimii kilpailutilanteessa. 

``cpp
//Create a Competition Object
competition Competition;

//Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Event has occurred");
}

int main() {
  // Register event with a callback function.
  Competition.drivercontrol(runOnEvent);

  while (true) {
    // Keep the main program running.
    wait(0.05, seconds);
  }
}
```
<advanced>
</advanced>