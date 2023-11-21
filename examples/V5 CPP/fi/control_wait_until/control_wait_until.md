category: control  
signature: while (!condition) {\n\n};  
description: Waits for a condition to return true before moving to the next command.

# Kun ei

Ohjauskomento jatkaa silmukan sisällä olevien komentojen suoritusta kunnes ehto toteutuu ja saa arvon **true**.

```cpp
while (!condition) {
  // Run some commands
}
```

## Miten käytetään

`while not` komento tarkistaa jokaisen silmukan  kierroksen alussa ehtoa ja siirtyy seuraavaan silmukan jälkeiseen komentoon vasta kun ehto saa arvon **true.**

Jos ehto on **false**, silmukan sisällä oleva koodi suoritetaan.

Jos ehto on **true**, silmukkan yli hypätään ja seuraava komento suoritetaan ja jatketaan siitä edelleen.

`while not` komento hyväksyy Boolean -lausekkeita, jotka voivat saada arvot 'True` tai `False`. Booleans tyyppisiä ehtoja ovat vertailuehdot ja loogiset operaatiot. 


`
```cpp
// Keep driving forward until the Bumper Pressing command returns true
while (!Bumper.pressing()) {
  Drivetrain.drive(forward);
}

// Stop the Drivetrain after the Bumper is pressed
Drivetrain.stop();
```

<advanced>
</advanced>