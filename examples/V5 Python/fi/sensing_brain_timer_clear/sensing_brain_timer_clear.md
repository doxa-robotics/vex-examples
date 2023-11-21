category: sensing  
signature: brain.timer.clear()  
description: Clears the V5 Brain's timer.

# Nollaa kello

Nollaa V5 Aivojen kellon.

```don 
brain.timer.clear()
```

## Miten käytetään

Aivojen kello käynnistyy ohjelman suorituksen alussa. Nollaa kello -komentoa voi käytttää ohjelman aikana aloiottaamaan ajanlasku uudelleen arvosta 0 sekuntia.

## Esimerkki

Ohjelman alussa kello nollataan. Ajopeli liikkuu eteenpäin 3 sekunnin ajan ja pysähtyy.

```don
brain.timer.clear()
while not brain.timer.time(SECONDS) > 3:
    drivetrain.drive(FORWARD)
drivetrain.stop()
```
	
<advanced>
</advanced>
