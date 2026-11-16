# Predloga modula

Predlogo kopirajte v novo datoteko in nadomestite navodila z vsebino. Pred vnosom preverite obstoječe datoteke v `MODULI/` in [indeks modulov](../MODULI.md): uporabite obstoječi modul, če že ustreza, sicer izberite prost identifikator. Obstoječe datoteke ne prepišite.

Identifikator in ime datoteke sta `NNN-MOD-naziv` in `NNN-MOD-naziv.md`. Za dejanske gradnike uporabljajte številke `001–899`, za primere izključno `900–999`. Številko izberite prosto znotraj vrste gradnika; med različnimi vrstami se lahko ponovi. Celoten identifikator mora biti enoličen.

Del `naziv` pišite z malimi črkami brez šumnikov in s presledki, zamenjanimi z vezaji. Pri primerih je obvezna izjema velika predpona `PRIMER-` pred tem delom; tudi prikazani naziv se začne s `PRIMER-`.

Na začetek vsakega primera dodajte opozorilo:

**PRIMER – Ta dokument je namenjen samo ponazoritvi strukture in uporabe. Ni del uradnega kurikuluma NIDiKo.**

Po vnosu dodajte povezavo »identifikator – naziv« v ustrezni razdelek indeksa. Pri preimenovanju poiščite stari identifikator in pot v vseh datotekah Markdown ter posodobite vse sklice.

Preverite skladnost ID z imenom datoteke, zaporedje učnih enot, veljavnost predpogojev in obstoj ciljnih datotek vseh relativnih povezav. Predloge ne vključujte v indeks.

## ID modula

Vnesite enoličen identifikator v obliki `NNN-MOD-naziv`.

## Naziv modula

Vnesite polni naziv modula.

## Opis

Opišite namen in vsebinsko povezanost modula, brez podvajanja opisov učnih enot.

## Ključne besede

Vnesite ključne besede, namenjene lažjemu iskanju modula.

## Seznam učnih enot

V urejenem seznamu navedite vsaj eno obstoječo učno enoto kot relativno povezavo v obliki `../UE/NNN-UE-naziv.md`; besedilo povezave naj bo »identifikator – naziv«.

Za vsako učno enoto določite tudi **predpogoje za vključitev v učno enoto**:

- **Brez predpogojev:** vpišite `brez`.
- **S predpogoji:** navedite enega ali več identifikatorjev učnih enot `NNN-UE-naziv`, ki jih mora udeleženec uspešno zaključiti pred vključitvijo v obravnavano učno enoto.

Predpogoji so neobvezni.

Upoštevajte naslednja pravila:

- Vsak predpogoj mora biti obstoječa učna enota.
- Učna enota ne sme biti sama sebi predpogoj.
- Če je predpogoj del istega modula, mora biti naveden pred odvisno učno enoto.
- Predpogoj je lahko tudi učna enota zunaj obravnavanega modula; v tem primeru ga označite kot zunanji predpogoj.
- Odvisnosti med učnimi enotami ne smejo biti krožne.
- Vrstni red učnih enot določa priporočeno zaporedje izvedbe, predpogoji pa obvezne pogoje za vključitev v posamezno učno enoto.
- Ista izvorna učna enota lahko nastopa v več različnih modulih.
- Predpogoji veljajo v kontekstu obravnavanega modula in se lahko med moduli razlikujejo.

### Primer zapisa

1. [900-UE-PRIMER-osnove-e-poste – PRIMER-Osnove e-pošte](../UE/900-UE-PRIMER-osnove-e-poste.md)
   - **Predpogoji:** brez

2. [901-UE-PRIMER-varna-raba-spleta – PRIMER-Varna raba spleta](../UE/901-UE-PRIMER-varna-raba-spleta.md)
   - **Predpogoji:** `900-UE-PRIMER-osnove-e-poste`

3. [902-UE-PRIMER-uporaba-spletnih-sestankov – PRIMER-Uporaba spletnih sestankov](../UE/902-UE-PRIMER-uporaba-spletnih-sestankov.md)
   - **Predpogoji:** `900-UE-PRIMER-osnove-e-poste`, `901-UE-PRIMER-varna-raba-spleta`

Pri ustvarjanju dejanskega modula primer zamenjajte s povezavami na izbrane učne enote in njihovimi predpogoji.