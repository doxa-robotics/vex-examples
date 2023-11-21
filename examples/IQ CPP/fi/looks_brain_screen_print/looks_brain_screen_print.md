category: looks  
signature: Brain.Screen.print("Hello");  
description: Prints values or text on the IQ Brain's screen.  

# Tulosta 

Tulostaa numeroarvoja tai tekstiä Aivojen näytölle.

```cpp
Brain.Screen.print();
```

## Miten käytetään

`Brain.Screen.print` komento tulostaa dataa näytön kursorin kohdalle näytöllä.

Kaikki uudet ohjelmat tulostaa kohtaan rivi 1 sarake 1.

Tulosta tekstiä:
```cpp
Brain.Screen.print("String: 123 + Words");
```

Tulosta kokonaisluku tai deimaalilukuja:
```cpp
// Kun tulostaa kokonaislukuja, käytetään "%d" formaattia
// ensimmäisenä parametrina

Brain.Screen.print("Integer: %d", 5 + 10);

// Kun tulostaa desimaalilukuja, käytetään "%f" formaattia
// ensimmäisenä parametrina

Brain.Screen.print("Decimal: %f", 5.0 + 10.0);
```

Tulosta sensoriarvo:
```cpp
// Kumpaa muotoa käytetään
// Kokonaisluvulle käytä"%f" tai desimaaaliluvulle käytä "%d" formaattia

Brain.Screen.print("%d", Brain.Timer.time());

// Boolean muuttujalle
// käytä "%s" formaattia

Brain.Screen.print("%s", Motor.isDone() ? "TRUE" : "FALSE");
```

<advanced>
</advanced>