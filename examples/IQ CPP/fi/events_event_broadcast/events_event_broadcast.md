category: events  
signature: EVENT.broadcast();  
description: Broadcast event message to run listener functions.

# Lähetä viesti

Lähettää viestin aktivoimaan tapahtumalla  **Event** toisen funktion.

```cpp
myEvent.broadcast();
```

## Miten käytetään

Pääohjelman koodi jatkuu heti kun komento `myEvent.broadcast` on lähetetty ts molemmat osat suoritetaan samaan aikaan.

Ennenkuin komentoa voi käyttää, käyttäjämääritelty tapahtuma pitää luoda ja rekisteröidä ainakin yhteen callback-funktioon.

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
  // Create an event in the main function
  event myEvent = event();

  // Register callback functions to event
  myEvent(runOnBroadcast1);
  myEvent(runOnBroadcast2);

  // Broadcast the event
  myEvent.broadcast();
}
```

<advanced>
</advanced>