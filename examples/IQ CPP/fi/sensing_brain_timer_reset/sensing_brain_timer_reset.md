category: sensing  
signature: sensing_brain_timer_reset 
description: Resets the Brain's timer.

# Nollaa kello

Nollaa aivojen kellon.

```cpp
Brain.Timer.reset();
```

## Miten käytetään

Aivojen kello käynnistyy kun ohjelma alkaa.`Brain.Timer.reset` käytetään nollaamaan kello.

## Esimerkki

Esimerkissä kello nollataan ennen kuin ajopeli ajaa 3 sekuntia eteenpäin, jonka jälkeen ajopeli pysähtyy.

```cpp
Brain.Timer.reset();
Drivetrain.drive(forward);

while (true) {
  if (Brain.Timer.value() > 3) {
    break;
  }

  wait(20, msec);
}

Drivetrain.stop();
```

<advanced>
</advanced>