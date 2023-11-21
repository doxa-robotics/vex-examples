category: control  
signature: for value in range (10): \n\tpass  
description: A type of loop that repeats the code contained inside for a set number of iterations. 

# Toista

Silmukkakomento, jossa koodia toistetaan annetun numeron mukainen määrä.

```don
for value in range(10):
    pass
```

# Miten käytetään

Ensiksi korvaa `value` muuttujalla , joka iteroidaan läpi `range()` funktion arvon.

Sitten korvaa  `10` arvolla , joka on iteraatiin lukumäärän loppuarvo.

Lisää komentoriveille aina 4 tyhjää osoittamaan , että rivit kuuluvat silmukan sisälle `for` ohjausrakenteessa.

for` komennnon sisällä ei saa olla tyhjää vaan lisää `pass` komento kutenedellä määritelty.

Huomaa että luuppi alkaa aina indeksillä 0.

`For` luuppeja voi laittaa toistensa sisään sisäkkäin.

# Esimerkki

Seuraava toista silmukka tulostaa luvut 0 lukuun 2 omille riveille:

```don
for i in range(3):
   brain.screen.print(i)
   brain.screen.new_line()
```
   
This will print:

```
0
1
2
```

<advanced>
</advanced>
