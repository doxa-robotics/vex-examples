category: functions  
signature: function_thread
description: Allows you to execute multiple threads at the same time.

# Ohjelmasäie

Antaa suorittaa useamman komentosäikeen samaan aikaan rinnakkain.

```cpp
thread myThread = thread(myThreadCallback);
```

## Miten käytetään

Pitää määritellä funktio, jota suoritetaan ohjelmasäikeenä.

```cpp
void myThreadCallback() {
  Brain.Screen.print("In a different thread!");
}
```
Kun funtio on määritelty, voit käyttää sitä toisena rinnakkaisena säikeenä. Funktiota kutsutaan ns **callback function** eli kutsufuntioksi.

```cpp
thread myThread = thread(myThreadCallback);
```
**thread** säie suoritetaan heti alussa samaan aikaan kuin pääohjelma (säie).

Vain **2 threads** säiettä kerrallaan vahva suositus. Lisäsäikeet voivat heikentää VEX IQ robotin suorituskykyä.
    
## Esimerkki

Tässä esimerkissä VEX IQ's aivoissa käytetään kahta kelloa yhtäaikaa eri säikeissä. Toisen tulostuksen hoitaa `myThread` säie. Toisen taas tulostaa pääohjelma main() säie yhtäaikaa.

```cpp
void myThreadCallback() {
  int count = 0;
  while(true) {
    Brain.Screen.setCursor(1, 1);
    Brain.Screen.print("thread1: %d", count);
    count++;
    // Odota että pääsäie suoritetaan
    wait(25, msec);
  }
}

int main() {
  // Kun säie on luotu aloita suoritus
  thread myThread = thread(myThreadCallback);
  
  int count = 0;
  while(true) {
    Brain.Screen.setCursor(2, 1);
    Brain.Screen.print("main: %d", count);
    count++;
    // Odota että myThread suoritetaan
    wait(25, msec);
  }
}
```

<advanced>
</advanced>
