# Predloga učne poti

Predlogo kopirajte v novo datoteko in nadomestite navodila z vsebino. Pred vnosom preverite obstoječe datoteke v `UCNE_POTI/` in [indeks učnih poti](../UCNE_POTI.md): uporabite obstoječo pot, če že ustreza, sicer izberite prost identifikator. Obstoječe datoteke ne prepišite.

Identifikator sestavljajo predpona `UP`, številka in obvezen kratek naziv, ločen z vezajem: `UPNNN-naziv`. Ime datoteke je identifikator s končnico `.md`, na primer `UP001-varno-sodelovanje.md`. Za dejanske gradnike uporabljajte številke `001–899`, za primere izključno `900–999`. Številko izberite prosto znotraj vrste gradnika; med različnimi vrstami se lahko ponovi. Številka mora biti enolična znotraj vrste gradnika tudi pri različnih kratkih nazivih.

Kratek naziv pišite z malimi črkami brez šumnikov in s presledki, zamenjanimi z vezaji. Pri primerih se prikazani polni naziv začne s `PRIMER-`; ta oznaka ni del identifikatorja.

Na začetek vsakega primera dodajte opozorilo:

**PRIMER – Ta dokument je namenjen samo ponazoritvi strukture in uporabe. Ni del uradnega kurikuluma NIDiKo.**

Po vnosu dodajte povezavo »identifikator – naziv« v ustrezni razdelek indeksa. Pri preimenovanju poiščite stari identifikator in pot v vseh datotekah Markdown ter posodobite vse sklice.

Preverite skladnost ID z imenom datoteke, zaporedje modulov, predpogoje in obstoj ciljnih datotek vseh relativnih povezav. Predloge ne vključujte v indeks.

## ID učne poti

Vnesite enoličen identifikator v obliki `UPNNN-naziv`; kratek naziv je obvezen.

## Naziv učne poti

Vnesite polni naziv učne poti.

## Opis

Opišite smiselno povezavo modulov v učno pot, brez podvajanja njihovih opisov.

## Ciljna skupina

Opišite, komu je učna pot namenjena.

## Ključne besede

Navedite ključne besede, namenjene lažjemu iskanju učne poti.

## Seznam gradnikov

V urejenem seznamu navedite vsaj en obstoječi modul ali učno enoto kot relativno povezavo v obliki `../MODULI/MNNN.md`, `../MODULI/MNNN-naziv.md`, `../UE/UINNN.md` ali `../UE/UINNN-naziv.md`; besedilo povezave naj bo »identifikator – naziv«.

Za vsak gradnik določite tudi **predpogoj za vključitev**:

- **Brez predpogoja:** vpišite `brez`.
- **S predpogojem:** navedite celoten identifikator obstoječega gradnika (`MNNN`, `MNNN-naziv`, `UINNN` ali `UINNN-naziv`), ki ga mora udeleženec uspešno zaključiti pred vključitvijo v obravnavani gradnik.

Predpogoj je neobvezen. Posamezen modul ali učna enota ima lahko največ en neposredni predpogoj.

**Pazite, da ne vzpostavite krožnih odvisnosti!**


### Primer zapisa

1. [M900-digitalna-komunikacija – PRIMER-Digitalna komunikacija](../MODULI/M900-digitalna-komunikacija.md)
   - **Predpogoj:** brez

2. [M901-varna-komunikacija – PRIMER-Varna komunikacija](../MODULI/M901-varna-komunikacija.md)
   - **Predpogoj:** `M900-digitalna-komunikacija`

Pri ustvarjanju dejanske učne poti primer zamenjajte s povezavami na izbrane module in njihovimi predpogoji.
