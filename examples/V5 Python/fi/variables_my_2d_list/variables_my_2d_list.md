category: variables  
signature: my_2d_list = [\n\t[0,0,0],\n\t[0,0,0],\n\t[0,0,0]\n]
description: 2D list variables are used to store multiple lists.

# 2D Taulukko

2D taulukkoon voi tallentaa useammalle riville ja sarakkeisiin arvoja.

## Miten käytetään

Nimeä 2D taulukko ja anna sille käyttöä kuvaava nimi .

Esimerkiksi 2d taulukkoon `coordinates` voi tallentaa useamman x,y koordinaatit.

Yksittäinen arvo annetaan symbolin `=` jälkeen hakasuluissa `[ ]`.

Hakasulkujen sisällä useammat arvot annetaan taas hakasuluissa pilkulla erotettuina: `[[ ], [ ]]`. More than two sets of square brackets can be nested within the outer-most set of square brackets.

Anna arvot hakasuluissa ja eroteltuna pilkulla `,`. Jos taulukko sisältää tekstikenttiä, laita ne lainausmerkkien `" "` sisään .

Jokainen sisempi hakasulku edustaa riviä. Rivin sisällä taas hakasulut merkkaavat 2d taulukon saraketta.

Kun haluat viitata johonkin alkioon taulukossa, anna taulukon nimi ja heti hakasuluissa rivin ja sarakkeen arvot. Ensimmäiset alkiot on aina indeksillä 0, ei 1.

Esimerkiksi 2D taulukko on määritelty coordinates = [[X1, Y1], [X2, Y2]]`, ja kun viitataan taulukon ensimmäiseen arvoon `coordinates[0][0]`, se palauttaa arvon `X1`. 

## Esimerkki 1

Esimerkissä 2d taulukkoon my_list on tallennettu kaksi erillistä värilistaa.

```don
my_list = [["Green", "Red", "Blue"], ["Black", "Yellow", "Orange"]]
```

## Esimerkki 2

Esimerkissä 2d taulukkoon my_list on tallennettu kaksi erillistä numerolistaa.

```don
my_list = [[1, 2, 3], [4, 5, 6]]
```
<advanced>
</advanced>
