category: events  
signature: EVENT.broadcast();  
description: Broadcast event message to run listener functions.<br /><br />A user defined event will need to replace the "EVENT" in this command.<br /><br />See the help listing for broadcast() for more information.  

# Tapahtuman lähetys

Lähettää tapahtumaviestin käynnistää vastaavan tapahtumafunktion.


```cpp
Event.broadcast();
```

## Miten käytetään

Ohjelma jatkaa suoritusta samaan aikaan kun `Event.broadcast();` komentoa suoritetaan kutsutun callback-funtion osalta.

Ennen kutsun käyttöä pitää tapahtuma olla määritelty ja rekistöröidä vastaava vähintää yksi callback-funtio.


```cpp
void runOnBroadcast1() {
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("Broadcast1 Running");
}

void runOnBroadcast2() {
  Brain.Screen.setCursor(2, 1);
  Brain.Screen.print("Broadcast2 Running");
}

int main() {
  // Create a new event.
  event myEvent;

  // Register callback functions to event.
  myEvent(runOnBroadcast1);
  myEvent(runOnBroadcast2);

  // Broadcast the event.
  myEvent.broadcast();
}
```

<advanced>
</advanced>