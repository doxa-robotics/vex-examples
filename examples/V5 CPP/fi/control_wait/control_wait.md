category: control  
signature: wait(time, seconds);  
description: Waits for a specific amount of time before moving to the next command.

# Odota

Odota tietty sekuntimäärä ennen seuraavan komennon suoritusta.

```cpp
wait(time, seconds);
```

## Miten käytetään

Aseta  sekuntimäärä time , kaunanko ohjelma odottaa seuraavaa komentoa.

```cpp
// Wait for 5 seconds before driving forward
wait(5, seconds);
Drivetrain.drive(forward);
```

<advanced>
</advanced>