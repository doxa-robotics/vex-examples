category: control  
signature: while expression: \n\tpass  
description: A loop that repeats the code while the condition returns true. 

# Kun

Silmukka , joka toistetaan niin kauan kuin sen ehto on voimassa ts **true**.   

```python
while condition:
    pass
```

## Miten käytetään

`while` silmukka tarkistaa sen ehdon aina jokaisen kierroksen alussa. 

Jos ehto on **true** (tosi), silmukan sisällä oleva koodi suoritetaan.

Jos ehto on **false** (epätosi), silmukan sisällä oleva koodi hypätään yli ja siirrytään seuraavaan komentoon.

`while` silmukka tarkastelee vain ehdon loogista arvoa joko `True` tai `False`. Ehdoksi voi sijoittaa minkä tahansa  Booleans -ehdon ilmaisun loogisen operaation tai vertailuoperaation. 

Voit käyttää yös nyúmeerisia arvolausekkeita ts arvo **0** merkitsee `False` ja muut **ei 0 numerot** merkistevät arvoa `True`. 

Lisää aina 4 tyhjää merkkiä *spacebar** rivin alkuun , jolla eroitat, mitkä komennot kuuluvat `while` silmukkaan mukaan. 

`while` komentoa ei saa sisältyy pelkkää tyhjää vaan silloin silmukan sisään tulee `pass` komento. 

## Esimerkki

Tässä `while` silmukassa tulsotetaan sana "Hello" uusille riveille kun aivojen kelloaika on alle 50 sekuntia.

```python
while brain.timer.time(SECONDS) < 50:
    brain.screen.print("Hello")
    brain.screen.next_row()
```

<advanced>
</advanced>
