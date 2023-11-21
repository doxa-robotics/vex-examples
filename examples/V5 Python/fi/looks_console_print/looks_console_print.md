category: looks  
signature: print("VEXcode")  
description: Prints values or text to the Print Console.  

# Konsoli tulostus

Tulostaa arvoja tai tekstiä tulostuskonsolille.

```python
print("VEXcode")
```

## Miten käytetään

`print` komento tulostaa dataa kursorikohtaan tulostuskonsolia.

Kaikki ohjelmat aloittavat aina kursorin rivin 1 kursorikohdasta.

## Rivitulostus

Oletuksen Python lisää aina uuden rivin `print` komennon jälkeen.

Jos haluat tulostaa useamman arvon riville käytä `end` parametria.

```python
print("This text will be ", end="")
print("printed on the same line")
```

## Arvojen tulostus

Voit käyttää Pythonissä `format` metodia muokataksesi tulostustmuotoa print komennossa.

Käytäessäsi `format` metodia, sinun pitää luoda peite/template tekstijono ja yhdistää osat aaltosuluilla - `{}`.

Kutsu `format` metodi template/muotoilu tekstijonossa. Jokainen parametri välitetään `format` method will be inserted into the replacement fields in sequence (if there are multiple replacement fields).

Voit lisätä muotoiluoptioita peite/template tekstijonoon asettamaan desimaalien lukumäärän. Jokainen formaaatttioptio alkaa aina kaksoispisteellä - `:`.

Esimerkissä Aivojen kello sijoitetaan yhteen korvaavaan kenttään template tekstijonossa ja se tulostetaan kahden desimaalin tarkkuudella.

```python
print("{:.2f}".format(brain.timer.time(SECONDS)))
```

Vastaavasti esimerkissä alla tulostetaan kursorin rivi/sarake arvo Aivoje näytölle. Korvauskenttien lukumäärä (suluissa `{}`) täytyy vastat parametrien määrää , jotka välitetään `format` metoodiin.

```python
# The value of brain.screen.row() will be passed into the first replacement field
# The value of brain.screen.column() will be passed into the second replacement field
print("Row: {:d}, Column: {:d}".format(brain.screen.row(), brain.screen.column()))
```

Tässä tyypilliset formaattitarkennuksia. Muitsa käyttää format tarkennuksia korvausmerkin sisällä (aaltosulkunen sisällä `{}`), ja seuraava merkki puolipiste- `:`.

* `d` - Desimaali / Kokonaisluku
* `f` - Liukuluku
* `o` - Oktaali kokonaisluku
* `s` - Tekstijono

Käyttämällä liukulukuformaattia `f`, voit määrittää desimaalien määrän.

* `.2f` - liukuluku 2 desimaalin tarkkuudella
* `.4f` - liukuluku 4 desimaalin tarkkuudella

## Tulostusvärit

Voit määrittää tulostusvärin tulostuskomennossa `print` .

Alla on kaksi eri tapaa määrittää tulostusväri. Kaikki värikoodit annetaan escape jonolla - `\033`.

* `[31m` - Red (punainen)
* `[32m` - Green (vihreä)
* `[34m` - Blue (sininen)
* `[30m` - Black (musta)
* `[37m` - White (valkoinen)
* `[33m` - Yellow (keltainen)
* `[91m` - Orange (oranssi)
* `[35m` - Purple (purppura)
* `[36m` - Cyan (syaani)
* `[97m` - Transparent (läpinäkyvä)

```python
# Using color codes in-line
# This will print "VEXcode" in Red to the Print Console
print("\033[31mVEXcode")

# Using color codes in separate commands
# Sets the print color for any subsequent prints
print("\033[31m")
print("VEXcode")
```

<advanced>
</advanced>
