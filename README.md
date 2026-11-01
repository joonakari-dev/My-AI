Sähkönkulutusta ennustava tekoäly

## Summary

Tämä projekti hyödyntää tekoälyä ja koneoppimista kotitalouden sähkönkulutuksen ennustamiseen ja optimointiin. Sen tavoitteena on auttaa käyttäjiä säästämään energiaa ja alentamaan kustannuksia älykkäiden suositusten avulla.

## Background

Sähkön hinnan voimakas vaihtelu ja energiatehokkuuden tärkeys ovat nousseet jokaisen kotitalouden arkeen. Monella kuluttajalla ei kuitenkaan ole selkeää kuvaa siitä, miten sähkönkulutus jakautuu tai miten sitä voisi ajoittaa fiksummin erityisesti pörssisähkön hintapiikkien aikana. Aihe on tärkeä, sillä se auttaa madaltamaan sähkölaskuja ja vähentämään kuormitusta sähköverkossa.

- Kotitalouksien vaikeus hahmottaa oman kulutuksensa huippukohtia
- Pörssisähkön hinnan arvaamaton vaihtelu tunnista toiseen
- Puuttuva helppokäyttöinen työkalu kulutuksen optimointiin arjessa

## How is it used?

Ratkaisua käytetään verkkosovelluksen kautta, josta kotitalous voi tarkastella seuraavan vuorokauden kulutusennustetta ja hintatietoja. Järjestelmä antaa suosituksia siitä, milloin on edullisinta käyttää raskaita kodinkoneita (kuten pesukonetta tai lattialämmitystä) tai ladata sähköautoa. Kohderyhmänä ovat tavalliset kuluttajat, jotka haluavat säästää rahaa vaivattomasti.
![Smart Home IoT](sebastian-scholz-nuki-IJkSskfEqrM-unsplash.jpg)
![Sähkönkulutuksen data-analyysi](ngital-8OYcY9CRP_0-unsplash.jpg)

## Data sources and AI methods
Projektissa hyödynnetään historiallista sähkönkulutusdataa sekä avoimia säätietoja (esim. lämpötilaennusteet, sillä ulkolämpötila vaikuttaa suoraan lämmityksen tarpeeseen). Mallin toteutuksessa käytetään koneoppimismalleja, kuten lineaarista regressiota.

| Syntax      | Description |
| ----------- | ----------- |
| Lämpötila   | Ulkolämpötilan vaikutus lämmitysenergian tarpeeseen |
| Vuorokauden aika | Kulutuksen vaihtelut arkena ja viikonloppuna |
Markdown
## Code example

Tässä on yksinkertainen esimerkki siitä, miten sähkönkulutusdataa voidaan käsitellä Pythonilla:

```python
# Esimerkki sähkönkulutuksen laskennasta
tunnit = [1, 2, 3, 4, 5]
kulutus_kwh = [1.2, 0.9, 0.8, 1.1, 2.5]

keskikulutus = sum(kulutus_kwh) / len(tunnit)
print(f"Keskimääräinen sähkönkulutus: {keskikulutus} kWh")


## Challenges

Tämä projekti ei ohjaa kodin sähkölaitteita automaattisesti, vaan tuottaa ennusteita ja suosituksia päätöksenteon tueksi. Tietosuojan osalta on tärkeää varmistaa, että kotitalouden tarkkoja kulutustietoja käsitellään turvallisesti.

## What next?

Tulevaisuudessa projektia voitaisiin laajentaa integroimalla se suoraan älykotijärjestelmiin (IoT), jolloin laitteet voisivat käynnistyä automaattisesti halpojen tuntien aikana. Tämä vaatisi lisäosaamista rajapintojen (API) käytöstä ja mobiilikehityksestä.

## Acknowledgments

- Fingridin avoin data ja sähkömarkkinatilastot
- Ilmatieteen laitoksen avoin säädata
- Building AI -kurssin opetusmateriaalit ja esimerkit
- [Smart Lock photo by Sebastian Scholz (Nuki)](https://unsplash.com/@nuki_smart_lock) on Unsplash
- [Laptop dashboard photo by ngital](https://unsplash.com) on Unsplash
