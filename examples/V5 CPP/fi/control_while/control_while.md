category: control  
signature: while(true) { }  
description: A loop that repeats the code inside the curly brackets while the condition returns true. 

# Kun

Koodi aaltosulkujen sisällä suoritetaan niin kauan kuun ehto saa arvon  **true**.   

```cpp
while (condition) {

}
```

## Miten käytetään

`while` luuppi tarkista ehdon vain aina kierroksen alussa ts aina koko aaltosulkujen sisällä oleva koodinpätkä suoritetaan. 


Jos ehto on **false**, `while` komento ohitetaan.

`while` komento hyväksyy Boolean ehtoja mm vertailuehtoja ja loogisia operaattoreita.Myös numeroarvoja ts arvo **0** vastaa **false** ja muut numerot **non-zero numbers** vastaa arvoa **true**. 

```cpp
// Drive forward while the timer value is less than 10 seconds

while(Brain.Timer.time(seconds) < 10) {
	Drivetrain.drive(forward);
}

Drivetrain.stop();
```

<advanced>
</advanced>