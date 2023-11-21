category: looks  
signature: print("\033[2J")  
description: Clears the Print Console.  

# Tyhjää konsoli

Tyhjää Tulostus konsolin.

```python
print("\033[2J")
```

## Miten käytetään

`print` komentoa käytetään `\033[2J` komentojonolla ja se tyhjää konsolin.

## Esimerkki

Esimerkisdsä tulostetaan sana "VEXcode" ja konsoli tyhjätään 3 sekunnin kuluttua.

```python
print("\033[31mVEXcode")

wait(2, SECONDS)

print("\033[2J")
```

<advanced>
</advanced>
