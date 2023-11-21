category: events  
signature: OPTICAL.objectDetected(callback);  
device_class: optical  
description: Runs the callback function when an object is detected by a V5 Optical Sensor  

# Optical löytää esineen

Suorittaa callback funktion kun V5 Optical Sensori havaitsee esineen/kohteen.


```cpp
Optical.objectDetected(callback);
```

## Miten käytetään

`optical.object_detected` komentoa voi käyttää triggeröimään haluttuja toimintoja kun V5 Optical Sensori havaitsee kohteen/esineen.

Sinun pitää luoda funktio, joka suoritetaan kun esine havaitaan. Anna funktiolle nimi , joka annetaan **callback** parametrissa ja suoritetaan kun esine havaitaan.

```cpp
// Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Object detected!");
}

int main() {
  // Register event with a callback function
  Optical.objectDetected(runOnEvent);
  
  while (true) {
    // Keep the main program running
    wait(0.05, seconds);
  }
}
```

<advanced>
</advanced>







