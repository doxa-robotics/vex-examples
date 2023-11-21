category: control  
signature: wait(time, units);  
description: Waits for a specific amount of time before moving to the next command.  

# odota

Odottaa asetetun ajan ennen kuin siirrytään seuraavaan komentoon.

```cpp
wait(time, units);
```

## Miten käytetään

Asettaa ajan joko **seconds** (sekuntia) tai **msec** (millisekunttia), jonka ohjelman suoritus odottaa ennen seuraavan komennon suoritusta ohjelmassa.

```cpp
wait(10, seconds);
wait(100, msec);
```

<advanced>
</advanced>