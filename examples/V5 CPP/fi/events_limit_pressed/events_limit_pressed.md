category: events  
signature: LIMIT.pressed(callback);  
device_class: limit  
description: Runs the specified function when the limit switch is pressed.<br /><br />A user defined callback will need to replace the "callback" parameter in order for this example snippet to compile.  

# Limit Switch painettu

Suoritetaan määritelty funktio kun Limit Switch painettu.

```cpp
LimitA.pressed(callback);
```

## Miten käytetään

Sensorin painallusta varten pitää määritellä funktio , jota kutsutaan painalluksen jälkeen. 

Anna funktiolle nimi ja määrittele sen toiminta, kun tapahtuma Limit Switch painettu . Kyseessä on ns `callback` parametri tapahtumalle.

``cpp
//Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Event has occurred");
}

int main() {
  // Register event with a callback function.
  LimitA.pressed(runOnEvent);

  while (true) {
    // Keep the main program running.
    wait(0.05, seconds);
  }
}
```

<advanced>
</advanced>