category: events  
signature: event myEvent = event(myEventCallback); 
description: Creates a new user event.

# Oma tapahtuma

Luo uuden oman tapahtuman triggeröimään käyttäjän määrittämä oma funktio.

```cpp
event myEvent = event(callbackFunction);
```

## Miten käytetään

**Event** tapahtumaobjektia käytetään kännistämään käyttäjän määrittelemä funktio. Jotta sitä voi käyttää, pitää, **event** tapahtumaobjekti luoda omalla nimellä. 


```cpp
event myEvent = event(callbackFunction);
```
Aina ei **Callback funktiota** tarvitse välittää luotuun tapahtumaan.

```cpp
event myEvent = event();
```
Useita **callback functioita** voi liittää samaan tapahtumaan. Kaikki kutsutut funktiot suoritetaan yhtäaikaaa kun tapahtuma sattuu ja niitä kutsutaan.

```cpp
event myEvent = event();
myEvent(callbackFunction1);
myEvent(callbackFunction1);
```
Mutta vain **2 event callback funktiota** voidaan suorittaa samanaikaisesti. Isompi määrä **events callback funktioita** voivat vaikuttaa VEX IQ robotin toimintakykyyn.

Callback funktio suoritetaan kun joko `myEvent.broadcast` tai `myEvent.broadcastAndWait` funktio suoritetaan.

## Callback Funktiot

Callback funktio on funktio, joka on välitetty toiselle funktiolle argumenttina. **Callback funktion** koodi suoritetaan kun haluttu **event** tapahtuma sattuu. 

```cpp
void callbackFunction() {
  Brain.Screen.print("Function Called.");
}

int main() {
  // Luo uusi tapahtuma nimeltään myEvent pääfunktiossa ja välitä callbackFunction tapahtumana myEvent = event(callbackFunction);

  // Lähetä myEvent, trggeroimaan "Function Called." jotta se tulostaa aivojen näytölle
  myEvent.broadcast();
}
```

<advanced>
</advanced>