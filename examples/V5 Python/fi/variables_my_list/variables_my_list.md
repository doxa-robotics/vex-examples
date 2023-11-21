category: variables  
signature: my_list = [0,0,0]  
description: List variables are used to store multiple values.  

# Luettelo muuttuja

Luetteloon voi tallentaa useampia muuttuja-arvoja.

## Miten käytetään

Anna luettelolle järkevä nimi . Hyvällä nimellä kuvaat luettelon käyttötarkoitusta.

esimerkiksi luettelonimi `colors` kuvaa sitä, että muuttujan alkiot ovat värien nimiä.

Kun haluat kohdisaa luettelon alkioon, käytä `=` operaattoria ja sen jälkeen arvot hakasuluissa `[ ]`.

Jos arvot ovat numeroita, eroita ne toisistaan pilkulla.

`my_number_list = [1, 2, 3]`

Jos arvot ovat tekstejä, niiden ympärillä pitää olla `" "` merkit ja pilkut eri alkioiden välillä.

`my_string_list = ["Hello", "World"]`

Jos haluat käyttää tiettyä luettelon alkion arvoa, nimen jälkeen hakasulkuihin alkion järjestysnumero , ensimmäinen alkio on järjestysnumerolla 0, ei 1.

Esimerkiksi `my_string_list[0]` palauttaa arvon `"Hello"`.

## Esimerkki 1

esimerkissä luetteloon my_list on tallennettu värien nimiä.

```don
my_list = ["Green", "Red", "Blue"]
```

## Esimerkki 2

Tässä esimerkissä taas luettelon my_list alkioihin on tallennettu numeroita.

```don
my_list = [1, 2, 3]
```

<advanced>
</advanced>
