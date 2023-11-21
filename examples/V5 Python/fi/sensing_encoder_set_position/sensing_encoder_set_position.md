category: sensing  
signature: encoder.set_position(POSITION, UNITS)
description: Sets the Shaft Encoder's position to the given value.

# Aseta akselianturin (kierrosmittarin) arvo
 
Asettaa akselianturille (kierrosmittarille) määrätyn arvon.

```python
encoder.set_position(POSITION, UNITS)
```

## Miten käytetään

Aseta encoder -anturin (kierrosmittarin) arvo sopivaan haluttuun positiiviseen lukuarvoon.

Yksikön 'UNITS` parametrina voi olla **DEGREES** (asteita) tai **TURNS** (kierroksia).

Tavallisesti encoder- kierrosmittari nollataan sopivassa kohtaan ohjelmaa.

<advanced>
</advanced>
