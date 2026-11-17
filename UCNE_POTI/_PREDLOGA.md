# Predloga učne poti

Predlogo kopirajte v novo datoteko in nadomestite navodila z vsebino. Pred vnosom preverite obstoječe datoteke v `UCNE_POTI/` in [indeks učnih poti](../UCNE_POTI.md): uporabite obstoječo pot, če že ustreza, sicer izberite prost identifikator. Obstoječe datoteke ne prepišite.

Identifikator in ime datoteke sta `NNN-UP-naziv` in `NNN-UP-naziv.md`. Za dejanske gradnike uporabljajte številke `001–899`, za primere izključno `900–999`. Številko izberite prosto znotraj vrste gradnika; med različnimi vrstami se lahko ponovi. Celoten identifikator mora biti enoličen.

Del `naziv` pišite z malimi črkami brez šumnikov in s presledki, zamenjanimi z vezaji. Pri primerih je obvezna izjema velika predpona `PRIMER-` pred tem delom; tudi prikazani naziv se začne s `PRIMER-`.

Na začetek vsakega primera dodajte opozorilo:

**PRIMER – Ta dokument je namenjen samo ponazoritvi strukture in uporabe. Ni del uradnega kurikuluma NIDiKo.**

Po vnosu dodajte povezavo »identifikator – naziv« v ustrezni razdelek indeksa. Pri preimenovanju poiščite stari identifikator in pot v vseh datotekah Markdown ter posodobite vse sklice.

Preverite skladnost ID z imenom datoteke, zaporedje modulov, predpogoje in obstoj ciljnih datotek vseh relativnih povezav. Predloge ne vključujte v indeks.

## ID učne poti

Vnesite enoličen identifikator v obliki `NNN-UP-naziv`.

## Naziv učne poti

Vnesite polni naziv učne poti.

## Opis

Opišite smiselno povezavo modulov v učno pot, brez podvajanja njihovih opisov.

## Ciljna skupina

Opišite, komu je učna pot namenjena.

## Ključne besede

Navedite ključne besede, namenjene lažjemu iskanju učne poti.

## Seznam gradnikov

V urejenem seznamu navedite vsaj en obstoječi modul ali učno pot kot relativno povezavo v obliki `../MODULI/NNN-MOD-naziv.md`; besedilo povezave naj bo »identifikator – naziv«.

Za vsak gradnik določite tudi **predpogoj za vključitev**:

- **Brez predpogoja:** vpišite `brez`.
- **S predpogojem:** navedite identifikator gradnika `NNN-MOD-naziv`, ki ga mora udeleženec uspešno zaključiti pred vključitvijo v ta modul.

Predpogoj je neobvezen. Posamezen modul ali učna enota ima lahko največ en neposredni predpogoj.

**Pazite, da ne vzpostavite krožnih odvisnosti!**


### Primer zapisa

1. [900-MOD-PRIMER-digitalna-komunikacija – PRIMER-Digitalna komunikacija](../MODULI/900-MOD-PRIMER-digitalna-komunikacija.md)
   - **Predpogoj:** brez

2. [901-MOD-PRIMER-varna-komunikacija – PRIMER-Varna komunikacija](../MODULI/901-MOD-PRIMER-varna-komunikacija.md)
   - **Predpogoj:** `900-MOD-PRIMER-digitalna-komunikacija`

Pri ustvarjanju dejanske učne poti primer zamenjajte s povezavami na izbrane module in njihovimi predpogoji.