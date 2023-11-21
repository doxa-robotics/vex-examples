category: control  
signature: control_if
description: Runs the code inside the if-statement's curly brackets, if the condition returns true. 

# Jos

If -Koodin aaltosulkulauseen sisällä olevat komennot suoritetaan jos ehto on tosi. 

```cpp
if (condition) {
  // koodi suoritetaan jos ehto on tosi 
}
```

## Miten käytetään

**if-statement** tutkii ehtoa vain kerran.

Jos ehto on tosi **true**, aaltosulkujen sisällä oleva koodi suoritetaan.

Jos ehto on epätosi **false**, aaltosulkujen sisällä olevan koodin yli hypätään.

```cpp
// Stop Motor1 if BumperA is pressed
if (BumperA.pressing()) {
  Motor1.stop();
}
```

<advanced>
</advanced>