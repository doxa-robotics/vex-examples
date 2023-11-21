category: events  
signature: LIMIT.released(callback);  
device_class: limit  
description: Runs the specified function when the Limit Switch is released.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Limit Switch vapautettu

Suoritetaan määritelty funktio kun Limit Switch vapautettu.

```cpp
LimitA.released(callback);
```

## Miten käytetään

Sensorin painallusta varten pitää määritellä funktio , jota kutsutaan vapautuksen jälkeen. 

Anna funktiolle nimi ja määrittele sen toiminta, kun tapahtuma Limit Switch vapautettu . Kyseessä on ns `callback` parametri tapahtumalle.

``cpp
//Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Event has occurred");
}

int main() {
  // Register event with a callback function.
  LimitA.released(runOnEvent);

  while (true) {
    // Keep the main program running.
    wait(0.05, seconds);
  }
}
```

<advanced>
</advanced>