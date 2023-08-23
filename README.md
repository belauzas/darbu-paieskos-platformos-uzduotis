# DARBŲ PAIEŠKOS PLATFORMA

## Užduoties esmė

Sukurti internetinę platformą, kur darbdaviai gali kelti darbo skelbimus. Realus pavyzdys galėtų būti https://www.cvbankas.lt

## Techniniai reikalavimai

-   README failas:
    -   instrukcijos kaip pasileisti programą
-   projektas sukeltas į Github
-   Frontend (FE) dalis pagaminta su: HTML, CSS/Bootstrap, JavaScript, React
-   Backend (BE) dalis pagaminta su: Node.js/Express.js, MySQL
-   TypeScript galima naudoti pasirinktinai
-   slaptažodžiai privalo būti šifruojami
-   Informacijos mainai tarp FE ir BE vyskta per REST API
-   Projektas privalo pasileisti ir veikti

## Projekto reikalavimai

-   tvarkingai atrodantis ir responsive dizainas
-   vartotojo sąsaja - SPA
-   formų duomenys validuojami ir turi aiškias/konkrečias klaidų žinutes

## Užduoties reikalavimai

Reikia sukurti tinklapį, turintį viešą ir administracinę sritis. Taip pat prisijungimo, registracijos ir atsijungimo patvirtinimo puslapius.

## Viešoji sritis

Pagrindiniame puslapyje turi būti atvaizduoti 6 naujausi darbo skelbimai bei papildomas mygtukas vedantis į visų darbo skelbimų puslapį. Kiekvienas darbo skelbimas turi turėti sekančius elementus:

-   pozicijos pavadinimą
-   kategorija
-   įmonės pavadinimą
-   įmonės logotipą
-   atlyginimą
-   darbo vieta (miestas, šalis)
-   prieš kiek laiko buvo įkeltas skelbimas, kurio galimi formatai:
    -   prieš [n] minučių
    -   prieš [n] valandų
    -   prieš [n] dienų
-   širdutė (like/unlike) ir jų kiekis (visų vartotojų pažymėtas kiekis):
    -   žymėti gali tik prisijungę vartotojai
    -   pilnas, vartotojo įsimintų darbo skelbimų sąrašas yra rodomas atskirame puslapyje

Skelbimų sąraše įrašai atvaizduojame koretelėmis bei viršuje pateikiant pačius naujausius skelbimus. Skelbimus galima atfiltruoti pagal skelbimų kategorijas, beirikiuoti pagal naujumą (tiek pilną sąrašą, tiek atfiltruotą sąrašą).

## Administracinė sritis: Administratorius

Svetainės administratorius turi turėti galimybę peržiūrėti visus įkeltus darbo skelbimus ir esant poreikiui juos užblokuoti ar atblokuoti. Administratorius tap pat turi turėti galimybę peržiūrėti darbdavių profilius ir esant poreikiui juos užblokuoti ar atblokuoti. Taip pat gali kurti ir redaguoti darbo skelbimų kategorijas. Pateikimas - lentelėmis.

Darbo skelbimų sąraše matomi elementai:

-   įmonės logotipas
-   įmonės pavadinimas
-   pozicijos pavadinimas
-   kategorija
-   atlyginimas
-   darbo vieta (miestas, šalis)
-   širdučių kiekis
-   veiksmų mygtukai: peržiūrėti, blokuoti/atblokuoti (priklauso nuo esamo blokavimo statuso), t.y. jei skelbimas nėra blokuotas, tai matomas blokavimo mygtukas, o jei skelbimas yra blokuotas, tai matomas atblokavimo mygtukas

Darbdavių sąraše matomi elementai:

-   įmonės logotipas
-   įmonės pavadinimas
-   darbo skelbimų kiekis (aktyvių ir blokuotų atskirai)
-   veiksmų mygtukai: peržiūrėti, blokuoti/atblokuoti (priklauso nuo esamo blokavimo statuso), t.y. jei skelbimas nėra blokuotas, tai matomas blokavimo mygtukas, o jei skelbimas yra blokuotas, tai matomas atblokavimo mygtukas
-   užblokavus darbdavį kartu niekur nebematoti ir jo sukurti darbo skelbimai, net jei jie individualiai ir nebuvo blokuoti

Darbo skelbimų kategorijų sąraše matomi elementai:

-   kategorijos pavadinimas
-   kategorijai priskirtų aktyvių darbo skelbimų kiekis
-   kategorijai priskirtų blokuotų darbo skelbimų kiekis

## Administracinė sritis: Darbdavys

Darbdavys turi turėti galimybę peržiūrėti visus savo įkeltus darbo skelbimus ir esant poreikiui juos peržiūrėti, redaguoti ir ištrinti. Pateikimas - lentelėmis.

Darbo skelbimų sąraše matomi elementai:

-   pozicijos pavadinimas
-   atlyginimas
-   darbo vieta (miestas, šalis)
-   širdučių kiekis
-   veiksmų mygtukai: peržiūrėti, aktyvuoti/paslėpti (priklauso nuo esamo aktyvumo statuso), t.y. jei skelbimas nėra aktyvus, tai matomas paslėpimo mygtukas, o jei skelbimas yra paslėptas, tai matomas aktyvavimo mygtukas

Jei darbo skelbimas buvo svetainės administratoriaus blokuotas, tai jis turi būti sąraše pateikiamas išskirtinai. Pateikiama eilutę atvaizduojant raudonu fonu ir nerodant galimų veiksmų mygtukų.

## Vertinimas:

<details open>
  <summary>1 balas - readme, dokumentacija, github</summary>
  
  ```
    -   0.5 balo - readme, dokumentacija
    -   commit'ų:
        -   0..39: 0 balo
        -   40..49: 0.3 balo
        -   50+: 0.5 balo
  ```
</details>

<details>
  <summary>1 balas - visų API validacijos</summary>
  
  ```
    -   0.1 balo - prisijungimo, registracijos, atsijungimo
    -   0.1 balo - širdučių
    -   0.5 balo - admin: darbdavių, darbo skelbimų ir jų kategorijų
    -   0.3 balo - darbdavio: darbo skelbimų
  ```
</details>

<details>
  <summary>1 balas - visų formų validacijos</summary>
  
  ```
    -   0.2 balo - prisijungimo forma
    -   0.2 balo - registracijos forma
    -   0.2 balo - naujo darbo skelbimo forma
    -   0.2 balo - darbo skelbimo redagavimo forma
    -   0.1 balo - naujos darbo skelbimo katogorijos forma
    -   0.1 balo - darbo skelbimo katogorijos redagavimo forma
  ```
</details>

<details>
  <summary>1 balas - duomenų bazės architektūra</summary>
  
  ```
    -   0.4 balo - vartotojai
    -   0.1 balo - token
    -   0.2 balo - darbo skelbimų kategorijos
    -   0.2 balo - darbo skelbimai
    -   0.1 balo - širdutės
  ```
</details>

<details>
  <summary>2 balas - administratoriaus sritis</summary>
  
  ```
    -   0.8 balo - darbdavių crud
    -   0.7 balo - darbo skelbimų crud
    -   0.5 balo - darbo kategorijų crud
  ```
</details>

<details>
  <summary>2 balas - darbdavio sritis</summary>
  
  ```
    -   1.5 balo - darbo skelbimų crud
    -   0.5 balo - admistratoriaus blokuoto skelbimo funkcionalumas
  ```
</details>

<details>
  <summary>2 balas - viešoji sritis</summary>
  
  ```
    -   0.5 balo - pagrindinis puslapis
    -   0.2 balo - prisijungimo puslapis
    -   0.3 balo - regitracijos puslapis
    -   0.5 balo - darbo skelbimų sąrašo puslapis
    -   0.5 balo - darbo skelbimo puslapis
  ```
</details>
