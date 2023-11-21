category: events  
signature: events_event_broadcast_and_wait   
description: Broadcast event message to run listener functions and wait for all listeners to finish before continuing.

# Lähetä viesti ja odota

Lähettää viestin aktivoimaan toivotun tapahtumafunktion tapahtuman **Event** , jolloin pääohjelma keskeytyy suorituksen ajaksi.

```cpp
myEvent.broadcastAndWait();
```

## Miten käytetään

`myEvent.broadcastAndWait` komento odottaa kaikkia viestejä, jotka kuuntelevat pyyntöä ennen jatkoa. Ja odota aiheuttaa pääohjelman seisahtumisen kunnes kutsutut funktiot on suoritettu loppuun.

Ennen komennon käyttöä pitää tapahtuma luoda ja ainakin yksi callback-funktio rekisteröidä.

## Callback funktiot

Callback funktio on funktio, joka välitetään argumenttina toiseen funktioon. **Callback function** sisällä oleva koodi suoritetaan kun haluttu **event** tapahtuma sattuu. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Function Called.");

  wait(5, seconds);
}

int main() {
  // Register a new event in the main function and pass the callbackFunction
  event myEvent = event(callbackFunction);

  // Broadcast the event and wait for it to finish executing
  myEvent.broadcastAndWait();

  // This will not run until the callbackFunction has completed execution
  Brain.Screen.newLine();
  Brain.Screen.print("Done!");
}
```

<advanced>
</advanced>