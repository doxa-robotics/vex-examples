category: control  
signature: control_waitUntil 
description: Waits for a condition to return true before moving to the next command.

# Odota kunnes

Toistaa koodisegmentin kunnes ehto **condition** antaa arvon tosi **true**.

```cpp
while (!condition) { 
  // Koodi toistetaan kunnes ehto toteutuu
}
```

## Miten käytetään

Kontrollimkomentoa tutkitaaan jatkuvasti ja ei -ehto  **not** suorittaa koodia kunnes ehto tosi **true** pysäyttää aaltosulkujen sisällä olevankoodin suorituksen.

```cpp
while (!TouchLED.pressing()) {
  wait(20, msec);
}
```

## Esimerkki 

Esimerkissä asetetaan  KosketusLED väriksi keltainen ja odotetaan kunnes KosketusLediä kosketetaan ja sen jälkeen Ledin valo muutetaan vihreäksi.

```cpp
TouchLED.setColor(yellow);

while (!TouchLED.pressing()) {
  wait(1, seconds);
}

TouchLED.setColor(green);
```

<advanced>
</advanced>