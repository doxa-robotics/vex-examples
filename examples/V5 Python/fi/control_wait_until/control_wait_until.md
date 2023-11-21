category: control  
signature: while not expression: \n\tpass  
description: A loop that continues until the expression turns true.  

# Kun ei

Ohjauskomento jatkaa silmukan sisällä olevien komentojen suoritusta kunnes Kun ehto toteutuu eli saa arvon **true**.

```python
while not condition:
    pass
```

## Miten käytetään

`while not` komento tarkistaa jokaisen silmukan  kierroksen alussa ehtoa ja siirtyy seuraavaan silmukan jälkeiseen komentoon vasta kun ehto saa arvon **true.**

Jos ehto on **false**, silmukan sisäll' oleva koodi suoritetaan.

Jos ehto on **true**, silmukan yli hyvätään ja seuraava komento suoritetaan ja jatketaan siitä edelleen.

`while not` komento hyväksyy Boolean -lausekkeita, jotka voivat saada arvot 'True` tai `False`. Boolean -tyyppisiä ehtoja ovat vertailuehdot ja loogiset operaatiot. 

Numeerisina arvoina käy **0** tarkoittaen `False`, ja mikä tahansa muu numeerinen arvo vastaa arvoa `True`. 

Lisää rivien alkuun 4 tyhjää merkkiä tarkoittaen että ne ovat osa silmuan sisällä olevia komentoja. 

`while not` silmukka ei saa olla tyhjä vaan lisää komento `pass` tarkoittanmaan ettei silmukassa tehdä mitään. 

## Esimerkki

`while not` silmukka tulostaa sanan "Hello" viisi kertaa kunnes muuttuja my_variable saa arvon 5.

```python
my_variable = 0

while not my_variable == 5:
    brain.screen.print("Hello")
    brain.screen.new_line()
    my_variable += 1
```

<advanced>
</advanced>
