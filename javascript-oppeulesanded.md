# JavaScripti ülesannete õpitee

See komplekt on üles ehitatud nii, et iga uus ülesanne kasutab vähemalt üht eelnevates töödes õpitud ideed edasi. Nii tekib loomulik areng lihtsast nupuvajutusest kuni väikese veebirakenduseni.

## Soovituslik järjekord

1. tervitaja
2. kalkulaator
3. parooli tugevuse kontrollija
4. registreerimisvorm
5. pildigalerii
6. kujunduse muutja
7. to-do list
8. JSON-andmete kuvamine
9. mini-ilmarakendus JSON-failist
10. AJAX-andmete laadimine
11. otsing ja filtreerimine
12. JavaScript vs jQuery
13. lõpuülesanne

---

## 1. "Tere, JavaScript" – nupud ja sündmused

**Eesmärk:** aru saada, kuidas HTML, CSS ja JavaScript koos töötavad.

**Õpilane teeb lehe, kus on:**
- pealkiri
- tekstiväli nime sisestamiseks
- nupp `Tervita`
- tulemusala, kuhu kuvatakse näiteks `Tere, Mari!`

**Harjutab:**
- muutujad
- `onclick` või `addEventListener`
- `document.querySelector`
- teksti muutmine lehel

**Seos järgmiste ülesannetega:**
- kasutaja sisendi lugemine
- nupu vajutuse käsitlemine
- tulemuse kuvamine lehel

---

## 2. Lihtne kalkulaator

**Eesmärk:** andmetüübid, operaatorid ja sisendi lugemine.

**Õpilane teeb kalkulaatori, kus kasutaja sisestab kaks arvu ja saab valida:**
- liitmine
- lahutamine
- korrutamine
- jagamine

**Lisatingimus:**
- kui jagatakse nulliga, kuvatakse veateade

**Harjutab:**
- arvutamine
- `Number()`
- tingimuslaused
- veakontroll

**Mida kasutatakse eelmisest edasi:**
- sisendväljade lugemine
- nupu sündmus
- tulemuse kuvamine DOM-is

---

## 3. Parooli tugevuse kontrollija

**Eesmärk:** vormid ja sisestuse valideerimine.

**Kasutaja sisestab parooli. Programm kontrollib, kas parool:**
- on vähemalt 8 märki pikk
- sisaldab numbrit
- sisaldab suurtähte
- sisaldab erimärki

**Tulemus kuvatakse näiteks kujul:**
- nõrk
- keskmine
- tugev

**Harjutab:**
- `if`
- stringid
- vormid
- valideerimine

**Mida kasutatakse eelmisest edasi:**
- kasutaja sisendi lugemine
- tingimuslaused
- tulemuse kuvamine dünaamiliselt lehel

---

## 4. Registreerimisvorm koos kontrollidega

**Eesmärk:** realistlik vormi valideerimise ülesanne.

**Vormis on väljad:**
- nimi
- e-post
- vanus
- parool
- parooli kordus

**Kontrollid:**
- kõik väljad peavad olema täidetud
- e-postis peab olema `@`
- vanus peab olema vähemalt 13
- paroolid peavad kattuma

**Harjutab:**
- vormid
- tingimuslaused
- kasutajale veateadete kuvamine

**Mida kasutatakse eelmisest edasi:**
- mitme sisendi kontrollimine korraga
- parooli valideerimise loogika
- selgete veateadete kuvamine kasutajale

---

## 5. Pildigalerii

**Eesmärk:** pildi lisamine ja `src` muutmine.

**Lehel on:**
- üks suur pilt
- mitu väikest eelvaatepilti

**Kui kasutaja klõpsab väiksel pildil:**
- suur pilt muutub

**Lisavõimalus:**
- nupp `Järgmine pilt`

**Harjutab:**
- pildi `src` muutmine
- sündmused
- DOM

**Mida kasutatakse eelmisest edasi:**
- klõpsu sündmused
- elementide leidmine `querySelector` abil
- sisu ja omaduste muutmine JavaScriptiga

---

## 6. Taustavärvi ja kujunduse muutja

**Eesmärk:** stiilide muutmine JavaScriptiga.

**Õpilane teeb lehe, kus saab valida:**
- hele või tume kujundus
- taustavärv
- fondi suurus

**Lisatingimus:**
- valikud salvestatakse `localStorage`-isse või küpsisesse
- järgmine kord jääb sama kujundus alles

**Harjutab:**
- CSS klasside muutmine
- `classList`
- `localStorage` või küpsised

**Mida kasutatakse eelmisest edasi:**
- nuppude ja valikute sündmused
- DOM-i muutmine
- kasutaja valikute rakendamine erinevatele elementidele

---

## 7. Lihtne to-do list

**Eesmärk:** dünaamilise sisu lisamine ja eemaldamine.

**Kasutaja saab:**
- lisada ülesande
- märkida ülesande tehtuks
- kustutada ülesande

**Lisavõimalus:**
- ülesanded salvestatakse `localStorage`-isse

**Harjutab:**
- massiivid
- DOM-elementide loomine
- sündmused
- andmete salvestamine

**Mida kasutatakse eelmisest edasi:**
- vormi sisendi lugemine
- salvestamine `localStorage`-isse
- klasside muutmine ja sündmuste haldus

---

## 8. JSON-andmete kuvamine

**Eesmärk:** JSON-i kasutamine andmeallikana.

**Näidisandmestik:**

```javascript
const students = [
  { name: "Mari", grade: 5 },
  { name: "Jüri", grade: 3 },
  { name: "Kati", grade: 4 }
];
```

**Ülesanne:**
- kuvada õpilased tabelis
- arvutada keskmine hinne
- näidata ainult neid, kelle hinne on vähemalt 4

**Harjutab:**
- JSON-i laadne andmestruktuur
- massiivid
- objektid
- tabeli genereerimine

**Mida kasutatakse eelmisest edasi:**
- dünaamiline HTML-i loomine
- andmete töötlemine enne kuvamist
- kasutajale tulemuste näitamine loetaval kujul

---

## 9. Mini-ilmarakendus JSON-failist

**Eesmärk:** andmete lugemine ja kasutajale kuvamine.

**Näidisandmestik:**

```json
[
  { "city": "Torva", "temperature": -2, "condition": "Pilves" },
  { "city": "Tallinn", "temperature": 1, "condition": "Lumine" }
]
```

**Lehel saab:**
- valida linna
- kuvada valitud linna temperatuur ja ilm

**Harjutab:**
- JSON
- valikukast
- andmete filtreerimine

**Mida kasutatakse eelmisest edasi:**
- objektide ja massiivide kasutamine
- andmete põhjal valikute loomine
- tulemuse kuvamine pärast kasutaja valikut

---

## 10. AJAX-andmete laadimine

**Eesmärk:** kliendi ja serveri vaheline asünkroonne andmevahetus.

**Õpilane teeb lehe, kus nupule vajutades laetakse andmed failist `data.json`:**
- kasutajad
- tooted
- uudised
- raamatud

**Lisatingimus:**
- andmeid ei kirjutata HTML-i käsitsi
- andmed tuuakse JavaScripti abil failist

**Harjutab:**
- `fetch()`
- AJAX-tehnika
- asünkroonne andmete laadimine

**Mida kasutatakse eelmisest edasi:**
- JSON-andmete kuvamine
- dünaamiline sisu loomine
- kasutaja tegevuse peale uute andmete näitamine

---

## 11. Otsing ja filtreerimine

**Eesmärk:** praktiline veebirakenduse osa.

**Lehel on toodete või filmide nimekiri. Kasutaja saab:**
- otsida nime järgi
- filtreerida kategooria järgi
- sortida hinna või nime järgi

**Harjutab:**
- massiivid
- `filter()`
- `sort()`
- sisendi jälgimine

**Mida kasutatakse eelmisest edasi:**
- JSON-ist või `fetch()` abil saadud andmete kuvamine
- dünaamiline nimekirja uuendamine
- kasutaja valikute sidumine andmete töötlemisega

---

## 12. jQuery võrdlusülesanne

**Eesmärk:** näha erinevust tavalise JavaScripti ja jQuery vahel.

**Õpilane teeb sama väikese funktsiooni kahel moel. Näiteks:**
- nupule vajutades peidetakse tekst
- nupule vajutades kuvatakse tekst tagasi
- lisatakse animatsioon

**Üks variant tehakse:**
- tavalise JavaScriptiga
- jQueryga

**Harjutab:**
- jQuery põhisüntaks
- erinevus tänapäevase JavaScriptiga

**Mida kasutatakse eelmisest edasi:**
- sündmused
- DOM-i muutmine
- klasside või stiilide vahetamine

**Õpetaja märkus:**
- see ülesanne sobib võrdlevaks harjutuseks pärast seda, kui õpilane oskab juba sama asja teha tavalise JavaScriptiga

---

## 13. Lõpuülesanne: lihtne veebirakendus

**Eesmärk:** siduda kokku kõik olulisemad teemad.

Valida võib ühe järgmistest variantidest.

### Variant A: Õpilaste hinnete haldur

**Funktsioonid:**
- lisa õpilane
- lisa hinne
- arvuta keskmine
- näita, kas hinne on positiivne
- salvesta andmed `localStorage`-isse
- laadi algandmed JSON-failist

### Variant B: Raamatukogu nimekiri

**Funktsioonid:**
- kuva raamatud JSON-ist
- otsi pealkirja järgi
- filtreeri žanri järgi
- märgi raamat loetuks
- salvesta kasutaja valikud

### Variant C: Lihtne e-pood

**Funktsioonid:**
- kuva tooted JSON-ist
- lisa ostukorvi
- arvuta kogusumma
- eemalda toode ostukorvist
- salvesta ostukorv `localStorage`-isse

**Mida kasutatakse eelmistest edasi:**
- vormid ja valideerimine
- dünaamiline DOM
- massiivid ja objektid
- `localStorage`
- JSON
- `fetch()`
- filtreerimine ja otsing

---

## Hindamiskriteeriumid

- leht töötab ilma JavaScripti vigadeta
- kasutaja sisestust kontrollitakse
- andmeid ei kirjutata kõik käsitsi HTML-i, vaid osa tuleb JavaScriptist või JSON-ist
- kood on loetav ja muutujate nimed on arusaadavad
- kujundus on lihtne, aga kasutatav
- lõpuülesandes on vähemalt üks asünkroonne andmelaadimine `fetch()` abil

---

## Miks see järjestus töötab

See järjekord liigub lihtsast keerulisemani:

1. kõigepealt õpitakse sündmusi ja sisendi lugemist
2. siis lisatakse tingimuslaused ja valideerimine
3. edasi hakatakse muutma DOM-i ja stiile
4. seejärel lisatakse andmete salvestamine
5. pärast seda minnakse massiivide, objektide ja JSON-i juurde
6. lõpuks kasutatakse `fetch()`-i, filtreerimist ja mitme osa ühendamist ühte rakendusse

Kõige loogilisem lühiversioonina on:

`tervitaja -> kalkulaator -> vormi valideerimine -> pildigalerii -> kujunduse salvestamine -> to-do list -> JSON -> AJAX -> otsing/filter -> lõpuülesanne`

