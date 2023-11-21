category: motion  
signature: motor.spin_to_position(POSITION, UNITS)
description: Spins a V5 Smart Motor to a certain position.

# Pyöritä asentoon

Pyörittää V5 Älymoottorin kierrosmittarin tiettyyn asentoon.

```python 
motor.spin_to_position(POSITION, UNITS)
```

## Miten käytetään

Komento kiertää moottorin asennon haluttuun kohtaan. Perustuu nykyiseen asentoon `spin_to_position` komento kertoo mihin suuntaan pyöritään että asento saavutetaan.

Valitse mittayksiköksi joko **DEGREES** (astetta) tai **TURNS** (kierroksia).

Optiona voit valita, odotetaanko komennon suoritus loppuun **wait=True** tai siirrytäänkö heti käännöksen aika seuraavaan komentoon  **wait=False**.

```python
motor.spin_to_position(90, DEGREES, wait=False)
```

Asettamalla **wait=True** tarkoittaa ,että ensin odotetaan se että moottori saavuttaa asetetun kohdan. Vastaavasti **wait=False** ei odota moottoorin pyörimistä tavoitteeseen ennen seuraavaa komentoa.  

Oletuksena on arvo **True**.

<advanced>
</advanced>
