# Leerlijnen ICT – OP STAP

Doorlopende leerlijnen ICT van kleuter tot 6de leerjaar, opgebouwd uit de 86 leerplandoelen ICT van Op.stap (leerplanversie V1.3, gecontroleerd op 29/10/2026) en de Leerlijn mediawijsheid van Mediawijs, aangevuld met de schooleigen AI-leerlijn van Scholengroep Sint-Rembert.

Deze versie is een naslagpagina: ze bewaart geen gegevens en vraagt geen aanmelding. Bij elk leerdoel opent de knop **✎ Suggestie** een e-mail naar rembertbasis.ict@sint-rembert.be.

## 1. Op GitHub Pages zetten

1. Maak op GitHub een nieuwe repository, bijvoorbeeld `leerlijnen-ict`.
2. Upload `index.html` en deze `README.md` (Add file > Upload files > Commit changes).
3. Ga naar **Settings > Pages**. Kies bij *Source* **Deploy from a branch**, branch **main**, map **/ (root)**, en klik **Save**.
4. Na een minuut staat de pagina op `https://<gebruikersnaam>.github.io/leerlijnen-ict/`.

Let op: een GitHub Pages-site is in de regel openbaar. Er staan geen persoonsgegevens in deze pagina.

## 2. Insluiten in SharePoint

1. Een SharePoint-beheerder voegt `github.io` toe aan de toegelaten domeinen: **Site-instellingen > HTML-veldbeveiliging** (anders blijft het venster leeg).
2. Bewerk een sitepagina, voeg het webonderdeel **Insluiten** toe en plak het adres van de GitHub-pagina.
3. Maak het webonderdeel zo hoog mogelijk of plaats het in een sectie op volle breedte. Een knop of link naar de pagina in een nieuw tabblad werkt ook altijd.

Rechtstreeks naar een leerjaar linken kan met `#yr-5de-leerjaar` achter het adres (ook `#yr-2de-kleuter`, `#yr-1ste-leerjaar`, enz.).

## 3. SharePoint-links toevoegen

De links staan in het aparte bestand `sharepoint-links.js`, zodat je `index.html` niet hoeft aan te raken.

1. Kopieer in SharePoint de link van een map: **Delen > Link kopiëren**.
2. Open op GitHub `sharepoint-links.js` en klik op het potloodje.
3. Zoek het leerdoel (per leerjaar gegroepeerd, met code en omschrijving erachter) en plak de link tussen de lege aanhalingstekens:
   `"5de-leerjaar_8-1-GL5-1": "https://…sharepoint.com/…",`
4. Klik **Commit changes**. Na een minuut verschijnt bij dat leerdoel de knop **Lesmateriaal in SharePoint ↗**, in de leerlijn én bij Per leerjaar.

Per leerjaar is er ook een regel `"map:5de-leerjaar"` voor de map van het hele leerjaar: die knop staat bovenaan bij Per leerjaar. Een lege regel geeft geen knop. Collega's hebben in SharePoint zelf toegang tot de map nodig; de links zijn zichtbaar op de openbare pagina, maar de mappen openen alleen voor wie toegang heeft.

## 4. Aanpassen

- Bewerk `index.html` op GitHub (potloodje) en klik **Commit changes**. GitHub bewaart elke versie.
- Bij een nieuwe versie van Op.stap: kijk het [wijzigingsoverzicht op PRO.](https://pro.katholiekonderwijs.vlaanderen/aanpassingen-aan-leerplan-sinds-1-september-2026-1) na en pas de leerdoelen, de dekkingscheck en de versie (bovenaan en bij Versiecontrole) aan.
