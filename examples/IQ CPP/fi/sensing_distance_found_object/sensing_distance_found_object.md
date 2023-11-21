category: sensing  
signature: Distance.foundObject()  
device-class: sonar
description: Reports if the VEX IQ Distance Sensor sees an object within its field of view. 

# Etäisyysanturi havaitsi esineen

Raportoi tiedon, havaitseeko VEX IQ Etäisyysanturi esineen näkökentässään. 

```cpp
Distance.foundObject()
```

## Miten käytetään

Antaa arvon **tosi**, jos se havaitsee esineen tai esinepinnan näkökentässään. 

Antaa arvon **epätosi**, jos se ei havaitse esinettä tai esinepintaa näkökentässään.

Ensinmmäisessä osassa annetaan nimetty etäisyysanturi, jota käytetään.

```cpp
Distance3.foundObject()
Distance4.foundObject()
```

## Esimerkki

Esimerkissä tulostetaan tieto aivojen näytölle, havaitseeko anturi esineen  tulostusarvoilla Ei tai Kyllä.

```cpp
Brain.Screen.print("Found Object: %s", Distance.foundObject() ? "Ei" : "Kyllä");
```

<advanced>
</advanced>