category: events  
signature: event Event = new event(); 
description: Create a new user-defined event.  

# Uusi tapahtuma

Luo uusi tapahtuma.

```cpp
event myEvent = event();

event myEvent;
```

## Miten käytetään

Käyttämällä allaolevaa syntaksia uusi käyttäjätapahtuma luodaan ennenkuin se toteuttava callback functio luodaan.

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
  // Create new events.
  event myEvent1 = event();
  event myEvent2;


  // Register callback functions to the events.
  myEvent1(runOnBroadcast1);
  myEvent2(runOnBroadcast2);

  // Broadcast the events.
  myEvent1.broadcast();
  myEvent2.broadcast();
}
```

<advanced>
</advanced>