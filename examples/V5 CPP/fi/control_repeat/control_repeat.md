category: control  
signature: repeat(10) { }  
description: Repeats the code inside curly brackets for a set number of times.

# Toista

Toistaa aaltosulkujen sisällä olevan koodin tietyn kertamäärän. 

```
repeat (10) {

}
```

## Miten käytetään

**repeat-statement** koodin sisöllä olevat koodirivit suoritetaan halutun kertamääärän ehdossa.

Arvo pitää olla positiivinen kokonaisluku, myös muuttujan tai sensorin arvo käy.

Ohessa sana "iteration" tulostetaan aivojen näytölle neljä kertaa. Joka kerralla tehdään myös uusi rivi.

```
repeat (4) {
  Brain.Screen.Print("iteration");
  Brain.Screen.newLine();
  wait(5, msec);
}
```

Huomaa ettei **repeat-statement** sisällä ei voi olla toista **repeat statement**.

<advanced>
</advanced>