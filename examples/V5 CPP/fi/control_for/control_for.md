category: control  
signature: for(int i = 0; i < length; i++) { }  
description: A type of loop that repeats the code contained inside for a set number of iterations. 

# Toista

Silmukkakomento, jossa koodia toistetaan annetun numeron mukainen määrä.

```cpp
for (initialization; condition; increment/decrement) {
   // code here will repeat a number of times
}
```

# Miten käytetään

Ensiksi anna arvo, joka kertoo montako kertaa silmukka toistetaan .

**for** komento tietää suorituksen aikana, montako kierrosta on mennyt:

* initialization on iterointimuuttujan alkuarvo, voit myös käyttää muuttujan arvoa 
* condition kertoo montako kertaa toisto tehdään. 
* increment/decrement expression kertoo iterointimuuttujan muuutoksen kierroksen lopussa
* 

Huomaa että luuppi alkaa aina indeksillä 0.

`For` luuppeja voi laittaa toistensa sisään sisäkkäin.

# Esimerkki

Seuraava toista silmukka tulostaa luvut 0 sta lukuun 9:

```cpp
for(int i = 0; i < 10; i++) {
   Brain.Screen.print(i);
   Brain.Screen.newLine();
}
```
<advanced>
</advanced>