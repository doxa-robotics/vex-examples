category: functions  
signature: function_thread
description: Allows you to execute multiple threads at the same time.

# Säikeet

Antaa suorittaa useamman säikeen yhtäaikaa.

```cpp
thread myThread = thread(myThreadCallback);
```

## Miten käytetään

Määrittele funktio ja tee callback kutsu säikeelle.

```cpp
void myThreadCallback() {
  Brain.Screen.print("In a different thread!");
}
```
Kun funktio on kirjoitettu, voi käyttää sitä uudelle säikeelle. Tätä kutsutaan  **callback funktioksi**.

```cpp
thread myThread = thread(myThreadCallback);
```
**thread** alkaa toimimaan heti, kun se on kirjoitettu. Se toimii yhtäaikaa kuin pääsäie.
    
## Esimerkki

Esimerkissä tulostetaan kaksi laskuriarvoa VEX V5 aivojen näytölle samaan aikaan. Toisen tulostaa thread säijeosa tekstin `myThread`. Toisen taas pääsäie samaan aikaan.

```cpp
void myThreadCallback() {
  int count = 0;
  while (true) {
    Brain.Screen.setCursor(1, 1);
    Brain.Screen.print("thread1: %d", count);
    count++;
    // Wait to allow the main thread to execute
    wait(25, msec);
  }
}

int main() {
  // Once a thread is created it begins executing
  thread myThread = thread(myThreadCallback);
  
  int count = 0;
  while (true) {
    Brain.Screen.setCursor(2, 1);
    Brain.Screen.print("main: %d", count);
    count++;
    // Wait to allow myThread to execute
    wait(25, msec);
  }
}
```

<advanced>
</advanced>
