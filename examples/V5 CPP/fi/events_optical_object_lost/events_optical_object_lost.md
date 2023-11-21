category: events  
signature: OPTICAL.objectLost(callback);  
device_class: optical  
description: Runs the callback function when a detected object is no longer being detected by a V5 Optical Sensor  

# Optical kohde hävisi

Ajetaan callback funktio, kun V5 Optical Sensori kadottaa äskeisen esineen.
```cpp
Optical.objectLost(callback);
```

## Miten käytetään

`optical.object_lost` komento käynnistää halutut toimenpiteet, kun V5 Optical sensori ei enää havaitse kohdetta/esinettä.

Luo funktio, jota kutsutaan kun esinettä ei enää havaita. Anna funktiolle nimi , joka kutsutaan, kun tapahtuma ilmenee **callback** parametrissa.


```cpp
// Function to run when the event occurs
void runOnEvent() {
  Brain.Screen.print("Object lost!");
}

int main() {
  // Register event with a callback function
  Optical.objectLost(runOnEvent);
  
  while (true) {
    // Keep the main program running
    wait(0.05, seconds);
  }
}
```

<advanced>
</advanced>







