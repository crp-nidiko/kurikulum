# Predloga modula

Predlogo kopirajte v novo datoteko in nadomestite navodila z vsebino. Pred vnosom preverite obstoječe datoteke v `MODULI/` in [indeks modulov](../MODULI.md): uporabite obstoječi modul, če že ustreza, sicer izberite prost identifikator. Obstoječe datoteke ne prepišite.

Identifikator sestavljajo predpona `M`, številka brez vodilnih ničel in kratek naziv z eno ali največ dvema ključnima besedama: `M1-naziv`. Ohranite izvorno številko modula iz Excela (`M1` → `M1-naprave`); pri uvozu uporabite identifikator in ime datoteke neposredno iz manifesta. Ime datoteke je identifikator s končnico `.md`, na primer `M1-naprave.md`. Za dejanske gradnike uporabljajte številke `1–899`; obstoječe demonstracijske primere s številkami `900–999` in njihovimi identifikatorji ohranite nespremenjene. Številka mora biti enolična znotraj vrste gradnika, med različnimi vrstami pa se lahko ponovi. Kratki del naj bo praviloma krajši od 20 znakov; polni naziv ostane nespremenjen.

Kratek naziv pišite z malimi črkami brez šumnikov in s presledki, zamenjanimi z vezaji. Pri primerih se prikazani polni naziv začne s `PRIMER-`; ta oznaka ni del identifikatorja.

Na začetek vsakega primera dodajte opozorilo:

**PRIMER – Ta dokument je namenjen samo ponazoritvi strukture in uporabe. Ni del uradnega kurikuluma NIDiKo.**

Po vnosu dodajte povezavo »identifikator – naziv« v ustrezni razdelek indeksa. Pri preimenovanju poiščite stari identifikator in pot v vseh datotekah Markdown ter posodobite vse sklice.

Preverite skladnost ID z imenom datoteke, zaporedje učnih enot, veljavnost predpogojev in obstoj ciljnih datotek vseh relativnih povezav. Predloge ne vključujte v indeks.

## ID modula

Vnesite enoličen identifikator v obliki `M1-naziv`, brez vodilnih ničel in s kratkim nazivom z eno ali največ dvema ključnima besedama. Pri uvozu uporabite identifikator iz manifesta.

## Naziv modula

Vnesite polni naziv modula.

## Opis

Opišite namen in vsebinsko povezanost modula, brez podvajanja opisov učnih enot.

## Ključne besede

Vnesite ključne besede, namenjene lažjemu iskanju modula.

## Seznam učnih enot

V urejenem seznamu navedite vsaj eno obstoječo učno enoto kot relativno povezavo v obliki `../UE/UE1-naziv.md`; besedilo povezave naj bo »identifikator – naziv«.

Za vsako učno enoto določite tudi **predpogoje za vključitev v učno enoto**:

- **Brez predpogojev:** vpišite `brez`.
- **S predpogoji:** navedite enega ali več identifikatorjev učnih enot `UE1-naziv`, ki jih mora udeleženec uspešno zaključiti pred vključitvijo v obravnavano učno enoto. Uporabite celoten identifikator obstoječe enote.

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

1. [UI900-e-posta – PRIMER-Osnove e-pošte](../UE/UI900-e-posta.md)
   - **Predpogoji:** brez

2. [UI901-spletna-varnost – PRIMER-Varna raba spleta](../UE/UI901-spletna-varnost.md)
   - **Predpogoji:** `UI900-e-posta`

3. [UI902-spletni-sestanki – PRIMER-Uporaba spletnih sestankov](../UE/UI902-spletni-sestanki.md)
   - **Predpogoji:** `UI900-e-posta`, `UI901-spletna-varnost`

Pri ustvarjanju dejanskega modula primer zamenjajte s povezavami na izbrane učne enote in njihovimi predpogoji.
