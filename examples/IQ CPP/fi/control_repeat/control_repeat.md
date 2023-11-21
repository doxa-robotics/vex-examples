category: control  
signature: repeat(10) { }  
description: Repeats the code inside curly brackets for a set number of times.

# Toista kertaa

Toistetaan ehdon sisällä aaltosuloussa olevat komennot suluissa oleva kertamäärä

`repeat (number of times to repeat){code to repeat}`

```
repeat (10) {

}
```

## Miten käytetään

**repeat-statement** toistaa aaltosuluissa olevat komenno normaalisuluissa olevan kertamäärän.

Ensiksi aseta kertamäärä toistolle , se voi olla myös kokonaislukumuuttuja tai vastaava sensoriarvo.

Koodipätkä alhaalla tulsotaa sanan "iteration" Aivojen näytölle 4 kertaa ja vaihtaa samalla riviä ennen seuraavaa kierrosta.

```
repeat (4) {
  Brain.Screen.print("iteration");
  Brain.Screen.newLine();
  wait(5, msec);
}
```

Huomioi että **repeat-statement** sisällä olevasta koodista ei voi siirtyä toiseen toisto komentoon.

<advanced>
</advanced>