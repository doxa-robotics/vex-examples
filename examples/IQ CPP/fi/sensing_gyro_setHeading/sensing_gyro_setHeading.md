category: sensing  
signature: Gyro.setHeading(heading, degrees);  
device_class: gyro  
description: Sets the Gyroscopic (Gyro) sensor's current heading to the value provided. 

# Gyro Aseta Ajosuunta

Asettaa Gyro Sensorin nykyisenajosuunnan tiettyyn arvoon. 

```cpp
Gyro.setHeading(heading, degrees);
```

## Miten käytetään

`Gyro.setHeading` komentoa voi käyttää asettamaan nykyisen ajosuunnan arvoon välillä **0** - **359.99**. 

Yleensä tätä käytetään asettamaan ajosuunta ohjelman keskellä arvoon 0.

`Gyro.setHeading` hyväksyy desimaali- ja kokonaislukuja.

## Esimerkki

Alla esimerkissä laitetaan Gyro Sensorin uusi ajosuunta arvoon 0 astetta.

```cpp
Gyro.setHeading(0, degrees);
```

<advanced>
</advanced>