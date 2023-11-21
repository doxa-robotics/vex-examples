category: variables  
signature: variables_2d_array
description: Declares the type, name, length of a 2D array. 

# 2D Taulukko Muuttuja

Määrittelee tyypin,nomen ja 2d taulukon koon ja antaa alkuarvot. 

```cpp
int my2DArray[3][3] = { 
  { 0, 1, 2 },
  { 3, 4, 5 },
  { 6, 7, 8 },
};
```

## Miten käytetään

Määrittele mitä tyyppiä 2d taulukkko on. 

- `int`
- `double`
- `bool`

Anna yksikäsitteinen nimi, joka kuvaa taulukkon käyttöä ja koko 2 parilla hakasulkuja `[]` heti nimen jälkeen. 

```cpp
// Declare a new 2D array with 3 rows and 3 columns

int my2DArray[3][3];
```

Oletusarvot taulukon alkiohin voi antaa aaltosuluissa yhtäläisyysmerkin jälkeen.

```cpp
int my2DArray[3][3] = { 
  { 0, 1, 2 },
  { 3, 4, 5 },
  { 6, 7, 8 }
};
```

Arvoja voi myös antaa indeksi kerrallaan, ensimmäinen indeksi on aina nolla. 

```cpp
// Declare a new turnAngles array with 3 rows and 3 columns
int turnAngles[3][3];

// Assign values by index
int turnAngles[0][0] = 45;
int turnAngles[0][1] = 90;
int turnAngles[0][2] = 180;
int turnAngles[1][0] = 270;
```

Kun arvoja käyttää, pitää haluttu alkio tarkentaa hakasuluilla.

```cpp
// The angle variable will be assigned the value of 270

int angle = turnAngles[1][0];
```

## Esimerkki

Tässä esimerkissä **desimaali** 2d taulukko`myAngles` sisältää kulma-asteita.

```cpp
double myAngles[2][3] = {
  {45.5, 90.0, 88.2},
  {25.0, 75.5, 45.0}
};
```

<advanced>
</advanced>