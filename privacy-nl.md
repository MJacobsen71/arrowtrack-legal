# Privacybeleid — JacArrow

**Laatst bijgewerkt:** 2026-05-20
**Verwerkingsverantwoordelijke:** Morten Jacobsen, Noorwegen
**Contact:** galge.vender.0a@icloud.com

---

## Korte versie

JacArrow slaat **al je data lokaal op je apparaat op**. We hebben geen
servers die je schoten, sessies of doelen ontvangen. Wanneer je
de app verwijdert, zijn alle data weg.

De enige derde partijen die informatie ontvangen, zijn:
- **Apple** — verwerkt App Store-aankopen en meldingen
- **RevenueCat** (na je Pro-aankoop) — verifieert je aankoop

Je hebt alle AVG-rechten op inzage, verwijdering en dataportabiliteit.

---

## Wat we opslaan

### Op je apparaat (lokaal, verlaat de telefoon nooit)
- **Schietdata:** sessies, rondes, pijlplaatsingen, scores, tags, doelen, bogen en pijlsets
- **Instellingen:** gekozen taal, thema, schiethand, wedstrijdklasse, meldingsopties
- **App-geschiedenis:** coach-mark-status (welke tips je hebt gezien), tutorial-voltooid-vlaggen

Al deze data worden opgeslagen in een SQLite-database en AsyncStorage op je iPhone.
Noch JacArrow noch een derde partij heeft toegang tot deze data.

### iCloud (alleen wanneer iCloud Drive is ingeschakeld)
JacArrow is van plan iCloud Key-Value Storage te gebruiken voor één specifiek doel:
onthouden of je de proefperiode eerder bent gestart. Dit synchroniseert
via je iCloud-account om te voorkomen dat verwijderen + opnieuw installeren
een nieuwe gratis proefperiode oplevert.

- Apple is de verwerker (onze overeenkomst valt onder hun standaardvoorwaarden)
- De opgeslagen waarden zijn **alleen**: de startdatum van de proefperiode en een «proef-gebruikt»-status
- Deze functie wordt geactiveerd zodra we het Pro-model lanceren (Fase 4b)

Als je iCloud Drive hebt uitgeschakeld, of iCloud Drive specifiek voor
JacArrow hebt uitgeschakeld, wordt iCloud niet gebruikt.

---

## Derde partijen

### Apple App Store
Alle in-app-aankopen worden afgehandeld door Apple. We ontvangen nooit kaartgegevens,
adressen of andere betalingsgegevens. Apples
[privacybeleid](https://www.apple.com/nl/legal/privacy/) is van toepassing op het
aankoopproces.

### Apple Push Notification Service (APNS)
JacArrow verstuurt lokale meldingen (PR behaald, einde proefperiode,
doelherinneringen). Om deze te bezorgen registreert iOS een anoniem apparaattoken
bij Apple. We hebben geen servers die push-berichten versturen — alle meldingen
worden lokaal op je apparaat gegenereerd op basis van de app-status.

### RevenueCat (alleen na Pro-aankoop)
Wanneer je JacArrow Pro koopt, registreert RevenueCat je bonnetje en een
anonieme `appUserId` (UUID gegenereerd op je apparaat). Dit is nodig om
de app je aankoop te laten verifiëren bij later gebruik en bij «Aankopen
herstellen». RevenueCats
[privacybeleid](https://www.revenuecat.com/privacy) is van toepassing. We sturen nooit
je naam, e-mail of andere persoonsgegevens.

### Apple Analytics / crashrapporten
Als je «App-analyse delen» hebt ingeschakeld in de iOS-instellingen, stuurt Apple
anonieme geaggregeerde data over gebruik en crashes naar de ontwikkelaar.
JacArrow gebruikt dit voor bugfixes en prestatie-optimalisatie. Je kunt
dit uitschakelen via:
**iOS-instellingen → Privacy en beveiliging → Analyse en verbeteringen**.

---

## Wat we NIET verzamelen

- Geen gebruikersaccount, e-mailadres of wachtwoord
- Geen GPS- of locatiegegevens
- Geen toegang tot contacten, agenda, camera of microfoon
- Geen trackers van derden (Firebase, Google Analytics, Facebook Pixel enz.)
- Geen advertentie-identificatoren (IDFA)
- Geen video-tracking of device fingerprinting

---

## Jouw rechten (AVG)

Je hebt de volgende rechten onder de Algemene Verordening Gegevensbescherming:

**Recht op inzage (Art. 15):** Al je data wordt lokaal op je apparaat opgeslagen.
Je hebt volledige inzage via:
- Instellingen → Mijn sessies (alle historische rondes)
- Instellingen → Mijn doelen (alle actieve en gearchiveerde doelen)
- Instellingen → Bogen / Pijlsets / Schietbanen (uitrustingsbeheer)

**Recht op dataportabiliteit (Art. 20):** Gebruik
**Instellingen → Mijn data exporteren** om al je data als JSON-bestand
te downloaden. Het bestand kan via het iOS-deelvenster gedeeld worden naar e-mail, AirDrop, Bestanden enz.
Dit is je complete schietgeschiedenis in een standaardformaat.

**Recht op wissen (Art. 17):**
- *Individuele sessie verwijderen:* veeg de sessie op het startscherm → Verwijderen
- *Alle data verwijderen:* deïnstalleer JacArrow — iOS verwijdert automatisch de hele
  SQLite-database en AsyncStorage. Het RevenueCat-bonnetje (als je
  Pro hebt gekocht) wordt door Apple en RevenueCat bewaard voor terugbetaling en support.

**Recht op beperking en bezwaar (Art. 18–21):** JacArrow neemt
geen geautomatiseerde beslissingen over jou. De Smart Insights-engine analyseert alleen
je eigen trainingsdata lokaal op je apparaat en presenteert
observaties — hij neemt geen beslissingen namens jou.

**Recht om toestemming in te trekken (Art. 7):** De opt-in voor Apple Analytics wordt
beheerd via de iOS-instellingen. RevenueCat-data wordt verwijderd wanneer je je Apple ID verwijdert.

---

## Wijzigingen

We werken dit beleid bij wanneer er belangrijke wijzigingen plaatsvinden in hoe we
data verwerken. Wijzigingen worden gecommuniceerd via:
1. De datum «Laatst bijgewerkt» bovenaan deze pagina
2. In-app-banner bij de eerste start na een update als de wijziging substantieel is
   (bijv. nieuwe derde partijen, nieuwe dataverzameling)

---

## Klachten

Als je vindt dat we je persoonsgegevens in strijd met de AVG verwerken,
heb je het recht om een klacht in te dienen bij je nationale gegevensbeschermingsautoriteit:

- **Nederland:** [Autoriteit Persoonsgegevens](https://autoriteitpersoonsgegevens.nl/)
- **EU/EER:** vind je autoriteit op
  [edpb.europa.eu](https://www.edpb.europa.eu/about-edpb/about-edpb/members_en)

We moedigen je aan eerst contact met ons op te nemen via galge.vender.0a@icloud.com — we nemen
alle privacyvragen serieus.
