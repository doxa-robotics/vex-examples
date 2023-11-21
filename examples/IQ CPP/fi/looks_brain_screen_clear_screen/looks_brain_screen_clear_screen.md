category: looks  
signature: Brain.Screen.clearScreen();  
description: Clears the entire V5 Brain screen.  

# Tyhjää näyttö

Tyhjää koko VEX IQ Aivojen näytön.

```cpp
Brain.Screen.clearScreen();
```

## Miten käytetään

`Brain.Screen.clearScreen` ei muuta kurssorin paikkaa näytöllä tyhjennyksen jälkeen. 

Käytä komentoa `Brain.Screen.setCursor` , jos haluat muuttuu kursorin paikkaa.

## Esimerkki

Esimerkissä tulostetaan "Hello", odotetaan sekunti ja putsataan koko näyttö ennen kuin tulostetaan "Goodbye".

```cpp
Brain.Screen.print("Hello");
wait(1.0, seconds);
Brain.Screen.clearScreen();
Brain.Screen.print("Goodbye");
```

<advanced>
</advanced>