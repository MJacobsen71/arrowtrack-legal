# Integritetspolicy — JacArrow

**Senast uppdaterad:** 2026-05-20
**Personuppgiftsansvarig:** Morten Jacobsen, Norge
**Kontakt:** galge.vender.0a@icloud.com

---

## Kort version

JacArrow lagrar **all din data lokalt på din enhet**. Vi har inga
servrar som tar emot dina skott, pass eller mål. När du avinstallerar
appen försvinner all data.

De enda tredje parter som tar emot information är:
- **Apple** — hanterar App Store-köp och notiser
- **RevenueCat** (efter att du köpt Pro) — verifierar ditt köp

Du har fullständiga GDPR-rättigheter till tillgång, radering och dataportabilitet.

---

## Vad vi lagrar

### På din enhet (lokalt, lämnar aldrig telefonen)
- **Skyttedata:** pass, omgångar, pilplaceringar, poäng, taggar, mål, bågar och pilset
- **Inställningar:** valt språk, tema, skytteshand, tävlingsklass, notisinställningar
- **App-historik:** coach-mark-status (vilka tips du har sett), tutorial-färdigflaggor

All denna data lagras i en SQLite-databas och AsyncStorage på din iPhone.
Varken JacArrow eller någon tredje part har tillgång till denna data.

### iCloud (endast när iCloud Drive är aktiverat)
JacArrow planerar att använda iCloud Key-Value Storage för ett specifikt syfte:
att komma ihåg om du har startat provperioden tidigare. Detta synkroniseras
via ditt iCloud-konto för att förhindra att avinstallation + ominstallation
ger en ny gratis provperiod.

- Apple är personuppgiftsbiträde (vårt avtal regleras av deras standardvillkor)
- Värdena som lagras är **endast**: provperiodens startdatum och en «prov-använd»-status
- Funktionen aktiveras när vi lanserar Pro-modellen (Fas 4b)

Om du har inaktiverat iCloud Drive, eller inaktiverat iCloud Drive specifikt
för JacArrow, används inte iCloud.

---

## Tredje parter

### Apple App Store
Alla köp i appen hanteras av Apple. Vi tar aldrig emot kortuppgifter,
adresser eller andra betalningsuppgifter. Apples
[integritetspolicy](https://www.apple.com/se/legal/privacy/) gäller för
köpflödet.

### Apple Push Notification Service (APNS)
JacArrow skickar lokala notiser (PR uppnått, provperiod löper ut,
målpåminnelser). För att leverera dessa registrerar iOS en anonym enhets-token
hos Apple. Vi har inga servrar som skickar push-meddelanden — alla notiser
genereras lokalt på din enhet baserat på appens tillstånd.

### RevenueCat (endast efter Pro-köp)
När du köper JacArrow Pro registrerar RevenueCat ditt kvitto och ett
anonymt `appUserId` (UUID genererat på din enhet). Detta krävs för
att appen ska kunna verifiera ditt köp vid senare användning och vid «Återställ
köp». RevenueCats
[integritetspolicy](https://www.revenuecat.com/privacy) gäller. Vi skickar aldrig
ditt namn, e-post eller andra personuppgifter.

### Apple Analytics / kraschrapporter
Om du har aktiverat «Dela app-analys» i iOS-inställningar skickar Apple
anonyma aggregerade data om användning och krascher till utvecklaren.
JacArrow använder detta för felrättning och prestandaoptimering. Du kan
inaktivera detta via:
**iOS-inställningar → Integritet och säkerhet → Analys och förbättringar**.

---

## Vad vi INTE samlar in

- Inget användarkonto, ingen e-postadress, inget lösenord
- Inga GPS- eller positionsdata
- Ingen åtkomst till kontakter, kalender, kamera eller mikrofon
- Inga tredjepartsspårare (Firebase, Google Analytics, Facebook Pixel m.fl.)
- Inga annonsidentifierare (IDFA)
- Ingen videospårning eller enhetsfingeravtryck

---

## Dina rättigheter (GDPR)

Du har följande rättigheter enligt dataskyddsförordningen:

**Rätt till tillgång (Art. 15):** All din data lagras lokalt på din enhet.
Du har full insyn via:
- Inställningar → Mina pass (alla historiska omgångar)
- Inställningar → Mina mål (alla aktiva och arkiverade mål)
- Inställningar → Bågar / Pilset / Banor (utrustningshantering)

**Rätt till dataportabilitet (Art. 20):** Använd
**Inställningar → Exportera mina data** för att ladda ner all din data som
JSON-fil. Filen kan delas via iOS delningsmeny till e-post, AirDrop, Filer m.fl.
Detta är din kompletta skyttehistorik i ett standardformat.

**Rätt till radering (Art. 17):**
- *Ta bort enskilt pass:* svep passet på startskärmen → Ta bort
- *Ta bort all data:* avinstallera JacArrow — iOS tar automatiskt bort hela
  SQLite-databasen och AsyncStorage. RevenueCat-kvitto (om du har
  köpt Pro) behålls hos Apple och RevenueCat för återbetalnings- och supportändamål.

**Rätt till begränsning och invändning (Art. 18–21):** JacArrow fattar
inga automatiserade beslut om dig. Smart Insights-motorn analyserar enbart
dina egna träningsdata lokalt på din enhet och presenterar
observationer — den fattar inga beslut å dina vägnar.

**Rätt att återkalla samtycke (Art. 7):** Apple Analytics opt-in styrs
via iOS-inställningar. RevenueCat-data raderas när du raderar ditt Apple-ID.

---

## Ändringar

Vi uppdaterar denna policy när väsentliga ändringar sker i hur vi behandlar
data. Ändringar kommuniceras via:
1. Datumet «Senast uppdaterad» högst upp på denna sida
2. In-app-banner vid första start efter uppdatering om ändringen är väsentlig
   (t.ex. nya tredje parter, ny datainsamling)

---

## Klagomål

Om du anser att vi behandlar dina personuppgifter i strid med GDPR har du
rätt att klaga till din nationella dataskyddsmyndighet:

- **Sverige:** [Integritetsskyddsmyndigheten (IMY)](https://www.imy.se/)
- **EU/EES:** hitta din myndighet på
  [edpb.europa.eu](https://www.edpb.europa.eu/about-edpb/about-edpb/members_en)

Vi uppmuntrar dig att kontakta oss först på galge.vender.0a@icloud.com — vi tar
alla integritetsfrågor på allvar.
