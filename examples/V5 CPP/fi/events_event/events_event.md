category: events  
signature: EVENT(callback);
description: Broadcast event message to run listener functions.<br /><br />A user defined event will need to replace the "EVENT" in this command.<br /><br />See the help listing for broadcast() for more information.  

# Tapahtuma rekistöröi callback funtion

Rekistöröi callback -function käynnistyksen kun käyttäjätapahtuma on annettu.

``cpp
Event(callback);
```

## Miten käytetään

Rekisteröi callback -funktio nimettyyn käyttäjätapahtumaan.

```cpp
void runOnBroadcast() {
  Brain.Screen.setCursor(1, 1);
  Brain.Screen.print("myEvent triggered runOnBroadcast callback");
}

int main() {
  // Create a new event.
  event myEvent;

  // Register a callback function to the myEvent event.
  myEvent(runOnBroadcast);

  // Broadcast the event.
  myEvent.broadcast();
}
```

<advanced>
</advanced>