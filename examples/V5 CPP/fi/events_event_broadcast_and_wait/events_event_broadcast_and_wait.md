category: events  
signature: EVENT.broadcastAndWait();    
description: Broadcast event message to run listener functions and wait for all listeners to finish before continuing.<br /><br />A user defined event will need to replace the "EVENT" in this command.<br /><br />See the help listing for broadcastAndWait() for more information.  

## Tapahtuman lähetys ja odota

Lähettää tapahtumaviestin käynnistää vastaavan tapahtumafunktion ja odottaa kunnes funktion toimenpiteet tehty.

```cpp
Event.broadcastAndWait();
```

## Miten käytetään

`Event.broadcastAndWait();` ohjelma odottaa kun komentoa suoritetaan kutsutun callback-funtion osalta. 

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

  // Broadcast the event and wait for completion.
  myEvent.broadcastAndWait();

  Brain.Screen.setCursor(3, 1);
  Brain.Screen.print("Listeners finished running");
}
```

<advanced>
</advanced>