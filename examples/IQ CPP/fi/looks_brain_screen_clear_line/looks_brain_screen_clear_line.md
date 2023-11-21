category: looks  
signature: Brain.Screen.clearLine();  
description: Clears a single row on the Brain screen.  

# Tyhjennä rivi

Tyhjentää halutun rivin VEX IQ aivojen näytöltä.

```cpp
Brain.Screen.clearLine();
```

Tyhjentää rivin 1  näytöllä.

```cpp
Brain.Screen.clearLine(1);
```

## Miten käytetään

`Brain.Screen.clearLine` tarvitsee kokonaisluvun rivinumeroksi väliltä **1 - 5**, mikä rivi tyhjätään. 

Jos rivinumeroa ei anneta, tyhjätään nykyinen rivi.

![row_column_index](row_column_index.png)  

## Esimerkki 
Esimerkissä tulostetaan "Hello" rivin 2 sarakkeeseen 1, odotetaan 3 sekuntia ja tyhjätään rivi 2.

```cpp
Brain.Screen.setCursor(2, 1);
Brain.Screen.print("Hello");
wait(3.0, seconds);
Brain.Screen.clearLine(2);
```

<advanced>
</advanced>