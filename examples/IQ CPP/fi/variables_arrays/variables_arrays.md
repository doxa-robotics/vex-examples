category: variables  
signature: variables_arrays
description: Declares the type, name, length of an array. 

# Taulukko/Luettelo Muuttuja

Määrittele tyyppi, nimi ja taulukon (luettelon) nimi. 

```cpp
int myArray[3] = { 1, 2, 3 };
```

## Miten käytetään

Määrittele minkä tyyppistä dataa taulukko sisältää. 

- `int`
- `double`
- `bool`

Taulukon nimi pitää olla yksikäsitteinen ja kuvaava. Aseta taulkukona lkioidern lukumäärä hakasuluissa `[]` heti nimen jälkeen. 

```cpp
int turnAngles[3];
```

Alkuarvot voi antaa heti taulukon luonnissa aaltosuluissa.

```cpp
bool boolArray[2] = { false, true };
```

Arvot voi myös antaa yksitellen indeksi kerrallaan indeksiarvosta 0 lähtien. 

```cpp
// Declare a new array of length 3
double doubleArray[3];

// Assign values to the array by index
double doubleArray[0] = 1.5;
double doubleArray[1] = 3.14;
double doubleArray[2] = 2.18;
```

Kun sijoitat taulukon arvoja johonkin, niin valitse indeksiarvo hakasuluissa.

```cpp
// Read the value at index 2 in integerArray

int value = integerArray[2];
```

## Esimerkki

Esimerkissä numerotaulukolle annetaan alkuarvot ja alkio #3 (indeksi arvo 2) sijoitetaan Moottorin kääntymiskulmaksi asteina. 

```cpp
int degreesArray[3] = { 30, 60, 90 };
Motor.spinFor(forward, degreesArray[2], degrees);
```

<advanced>
</advanced>