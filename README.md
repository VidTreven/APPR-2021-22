# Analiza podatkov s programom R - 2021/22
# Analiza slovenskih statisticnih regij glede na kakovost zivljenja v letih 2011 - 2020

Avtor: Vid Treven

Repozitorij za projekt pri predmetu APPR v študijskem letu 2021/22. 

## Tematika

Pri projektni nalogi bom raziskal slovenske statisticne regije v letih 2011 - 2020.
Cilj naloge je, da bom iz izbanih podatkov lahko izbral regijo, v kateri bi najraje zivel.
Za vsako regijo bom izbral podatke o pocutju tamkajsnjih prebivalcev, 
njihovem financnem stanju, zivorodnosti, vzrokih smrti, kriminaliteti,
onesnazenosti, pa tudi na tamkajsnje vreme ne bom pozabil.

## Viri

* Pocutje prebivalcev: [linked phrase](https://pxweb.stat.si/SiStatData/pxweb/sl/Data/-/0872040S.px)
* Financno stanje: [linked phrase](https://pxweb.stat.si/SiStatData/pxweb/sl/Data/-/0868140S.px)
* Zivorojeni: [linked phrase](https://pxweb.stat.si/SiStatData/pxweb/sl/Data/-/05J2008S.px)
* Vzrok smrti: [linked phrase](https://pxweb.stat.si/SiStatData/pxweb/sl/Data/-/05L3016S.px)
* Kriminaliteta: [linked phrase](https://pxweb.stat.si/SiStatData/pxweb/sl/Data/-/1372202S.px)
* Onesnazevanje: [linked phrase](https://pxweb.stat.si/SiStatData/pxweb/sl/Data/-/2706105S.px)
* Podnebje (Vreme): [linked phrase](https://meteo.arso.gov.si/met/sl/archive/)

## Izdelava

Naredil bom tabelo, ki bo imela 12 (regij) x 120 (mesecev) vrstic in 26 stolpcev.
Stolpci bodo:
* Regija
* Leto
* Mesec
* Splosno zadovoljstvo (4 stolpci)
* Prezivetje s prihodki (6 stolpcev)
* Zivorodnost (2 stolpca)
* Vzrok smrti (1 stolpec)
* Obsojeni (2 stolpca)
* Komunalni odpadki (3 stolpci)
* Podnebje (5 stolpcev)

Opomba: Pri podnebju si bom pogledal povprecno max in min temperaturo, kolicino padavin, 
stevilo dni z nevihto in stevilo dni s snezno odejo.

## Program

Glavni program in poročilo se nahajata v datoteki `projekt.Rmd`.
Ko ga prevedemo, se izvedejo programi, ki ustrezajo drugi, tretji in četrti fazi projekta:

* obdelava, uvoz in čiščenje podatkov: `uvoz/uvoz.r`
* analiza in vizualizacija podatkov: `vizualizacija/vizualizacija.r`
* napredna analiza podatkov: `analiza/analiza.r`

Vnaprej pripravljene funkcije se nahajajo v datotekah v mapi `lib/`.
Potrebne knjižnice so v datoteki `lib/libraries.r`
Podatkovni viri so v mapi `podatki/`.
Zemljevidi v obliki SHP, ki jih program pobere,
se shranijo v mapo `../zemljevidi/` (torej izven mape projekta).
