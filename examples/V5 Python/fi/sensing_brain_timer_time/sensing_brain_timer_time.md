category: sensing  
signature: brain.timer.time(UNITS)  
description: Reports the value of the V5 Brain's timer in the provided UNITS.

# Kellon aika

Raportoi V5 Aivojen kellon ajan halutussa yksikössä UNITS.

```python
brain.timer.time(UNITS)
```

## Miten käytetään

Kello käynnistyy ajasta 0 ohjelman alussa ja antaa ajan desimaalilukuna.

`UNITS` parametrina voi käyttää joko **SECONDS** tai **MSEC** (millisekuntia).

```python
while True:
    brain.screen.clear_screen()
    brain.screen.set_cursor(1, 1)
    brain.screen.print("Timer in Seconds: ", brain.timer.time(SECONDS))

    # A brief wait to print values without distortion or tearing
    wait(20, MSEC)
```
	
<advanced>
</advanced>
