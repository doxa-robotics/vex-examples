category: sensing  
signature: distance.object_size()  
description: Reports the size of an object using Distance sensor.

# Kohteen koko

ANtaa kohteen koon, jonka etäisyysanturi havaitsee.  

```
distance.object_size()
```

## Miten käytetään

Määrittää havaitun esineen koon (ei löydy, pieni,keskivertyo,laaja) perustuen valon määrään, joka heijastuu takaisin anturiin.


Jos j´kode löytyy , kunktio palauttaa `ObjectSizeType.SMALL`, `ObjectSizeType.MEDIUM`, tai `ObjectSizeType.LARGE`.

Jos kohdetta ei löydy, funktio palauttaa 'ObjectSizeType.NONE`.
	
<advanced>
</advanced>
