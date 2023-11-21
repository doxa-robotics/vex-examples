category: sensing  
signature: optical.color()
description: Reports the color that the Optical Sensor is detecting.


# Optical havaitsee värin

ANtaa värin, jonka Optical Sensori havaitsee.

```don
optical.color()
```

## Miten käytetään

`optical.color()` antaa RGB (Red, Green, Blue) -arvon, joka vastaa väriä. Voit käyttää funktiota `Color` eri arvoja ja vertailla sitä `optical.color()` sensorin antamaan arvoon

Voit vertailla värien arvot seuraavasti

* Color.BLACK (musta)
* Color.WHITE (valkoinen)
* Color.RED (punainen)
* Color.GREEN (vihreä)
* Color.BLUE (sininen)
* Color.YELLOW (keltainen)
* Color.ORANGE (oranssi)
* Color.PURPLE (purppura)
* Color.CYAN (syaani)

Voit käyttää ehtoja seuraavasti:

```don
if optical.color() == Color.RED:
	brain.screen.print("Red Object")
```

<advanced>
</advanced>