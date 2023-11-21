category: events  
signature: competition Competition = competition();
description: Create a new competition instance.

# Uusi kilpailu

Luo uusi kilapilu ilmentymä (ohjelma).

```cpp
competition Competition = competition();

competition Competition;
```

## Miten käytetään

Luo uusi kilpailu ilmentymä ottamalla ohjelmaan mukaan **driver_control** ja **autonomous** callback -funktiot.

Kun **driver control** signaali kilpailukytkimestä saadaan, niin suoritetaan **driver_control** callback funktio.

Vastaavasti, kun **autonomous** signaali kilpailukytkimestä saadaan, niin suoritetaan **autonomous** callback funktio.

`
```cpp
// Create a new Competition instance
competition Competition;

// Function to run when the "autonomous" signal is received
void runOnAutonomous() {
  Brain.Screen.print("Running autonomous");
}

// Function to run when the "driver control" signal is received
void runOnDriverControl() {
  Brain.Screen.print("Running driver control");
}

int main() {
  // Register competition event with callback functions.
  Competition.autonomous(runOnAutonomous);
  Competition.drivercontrol(runOnDriverControl);

  while (true) {
    // Keep the main program running.
    wait(0.05, seconds);
  }
}
```

<advanced>
</advanced>