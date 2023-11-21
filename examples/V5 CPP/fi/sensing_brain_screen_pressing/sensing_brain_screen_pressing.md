category: sensing  
signature: Brain.Screen.pressing()  
description: Reports if the V5 Brain's touchscreen is currently being pressed.

# Näyttöä koskettu
 
Antaa tiedon jos V5 aivojen kosketusnäyttöä on koskettu.

```cpp
Brain.Screen.pressing()
```

## Miten käytetään

`Brain.Screen.pressing()` komentoa voi käyttää yhdessä komentojen `Brain.Screen.xPosition()` ja `Brain.Screen.yPosition()` , jos V5 aivojen kosketusnäyttöä on koskettu ja missä kohtaan.

`Brain.screen.pressing()` antaa arvon **True** jos V5 aivojen näyttöä on koskettu.

`Brain.screen.pressing()` antaa arvon **false** jos V5 aivojen näyttöä ei ole koskettu.

```cpp
if (Brain.Screen.pressing()) {
  Brain.Screen.print("Screen is being pressed!");
}
```


<advanced>
</advanced>