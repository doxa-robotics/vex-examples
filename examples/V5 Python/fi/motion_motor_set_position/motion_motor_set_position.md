category: motion  
signature: motor.set_position(0, UNITS)  
description: Sets the V5 Smart Motor's encoder position to the given value.  

# Aseta moottorin asento

Asettaa V5 Älymoottorin kierrosasennon (encoderin) asennon annettuun arvoon.

```python
motor.set_position(VALUE, UNITS)
```

## Miten käytetään

Komento sallii positiivisia arvoja.

Tyypillisesti komennolla nollataan asento kesken ohjelmaa.

Komento `motor.set_position` hyväksyy sekä **DEGREES** (asteita) tai **TURNS** (kierroksia) yksikköinä **UNITS**.

<advanced>
</advanced>
