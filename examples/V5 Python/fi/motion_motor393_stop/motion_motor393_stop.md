category: motion  
signature: motor393.stop()  
description: Stops a Motor393 connected to a Motor Controller 29.

# Pysäytä Servo Ohjaus

Pysäyttää moottorin Motor393 , jota hallitsee Moottori Controller 29.

```python
motor393.stop()
```

## Miten käytetään

Esimerkissä Motor393 pysäytetään, kun ensin pyörinyt 3 s.

```python
motor393.spin(FORWARD)
wait(3, SECONDS)
motor393.stop()
```

<advanced>
</advanced>
