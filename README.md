# NIDiKo – Prilagodljivi kurikulum digitalnih kompetenc

V okviru raziskovalnega projekta NIDiKo nastaja prilagodljivi kurikulum neformalnega izobraževanja na področju digitalnih kompetenc. Repozitorij je namenjen opisovanju in povezovanju učnih enot, modulov in učnih poti v dokumentih Markdown.

## Struktura kurikuluma

**Učna pot → Gradnik (Modul → Učna enota) ali Učna enota**

Učne enote sestavljajo module, moduli pa učne poti. Ista učna enota lahko nastopa v več modulih in isti modul v več učnih poteh; vsak gradnik ima eno izvorno datoteko, drugi se nanjo sklicujejo s povezavo. Izjemoma lahko v učni poti nastopa tudi posamezna učna enota.

## Identifikatorji in imena datotek

- **Učna enota:** `UE` + številka brez vodilnih ničel + kratek naziv z eno ali največ dvema ključnima besedama, npr. `UE1-racunalnik`.
- **Modul:** `M` + številka brez vodilnih ničel + kratek naziv z eno ali največ dvema ključnima besedama, npr. `M1-naprave`.
- **Učna pot:** `UP` + številka + obvezen kratek naziv, npr. `UP001-varno-sodelovanje`.

Predpona in številka sta zapisani skupaj. Kratek naziv sledi vezaju, uporablja male črke brez šumnikov in vezaje namesto presledkov. Ime datoteke je celoten identifikator s končnico `.md`; v povezavah in predpogojih uporabljajte celoten identifikator, vključno s kratkim nazivom. Pri modulih in učnih enotah ohranite izvorno številko iz Excela, kratki del naj bo praviloma krajši od 20 znakov, polni nazivi pa ostanejo nespremenjeni. Pri uvozu uporabite številke in kratke nazive iz manifesta; za učne enote uporabite predpono `UE` tudi, če manifest še vsebuje predpono `U`.

Za dejanske module in učne enote so namenjene številke `1–899`, za primere `900–999`. Poimenovanje učnih poti ostane nespremenjeno. Obstoječi primeri ohranijo dosedanje identifikatorje in imena datotek (npr. `UI900-e-posta`). Številka mora biti enolična znotraj vrste gradnika, med vrstami pa se lahko ponovi. Oznaka `PRIMER-` ostane v prikazanem polnem nazivu primera in ni del identifikatorja. Podrobna navodila so v predlogah [učne enote](UE/_PREDLOGA.md), [modula](MODULI/_PREDLOGA.md) in [učne poti](UCNE_POTI/_PREDLOGA.md).

## Katalogi

- [Učne enote](UCNE_ENOTE.md)
- [Moduli](MODULI.md)
- [Učne poti](UCNE_POTI.md)

## Projekt

- [Projektna spletna stran NIDiKo](https://crp-nidiko.github.io/)
- [Uradna predstavitev projekta](https://ii.feri.um.si/sl/raziskovanje/raziskovalni-projekti/nidiko/)
