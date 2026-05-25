# Privatlivspolitik — JacArrow

**Sidst opdateret:** 2026-05-25
**Dataansvarlig:** Morten Jacobsen, Norge
**Kontakt:** galge.vender.0a@icloud.com

---

## Kort version

JacArrow gemmer **alle dine data lokalt på din enhed**. Vi har ingen
servere, der modtager dine skud, pas eller mål. Når du afinstallerer
appen, forsvinder alle data.

De eneste tredjeparter, der modtager information, er:
- **Apple** — håndterer App Store-køb og notifikationer
- **RevenueCat** (efter du har købt Pro) — verificerer dit køb
- **Sentry** (kun hvis du aktiverer nedbrudsrapporter) — modtager anonyme nedbrudsdata, så vi kan rette fejl

Du har fulde GDPR-rettigheder til indsigt, sletning og dataportabilitet.

---

## Hvad vi gemmer

### På din enhed (lokalt, forlader aldrig telefonen)
- **Skydedata:** pas, runder, pilplaceringer, point, tags, mål, buer og pilset
- **Indstillinger:** valgt sprog, tema, skydehånd, konkurrenceklasse, notifikations-indstillinger
- **App-historik:** coach-mark-status (hvilke tips du har set), tutorial-fuldført-flag

Alle disse data gemmes i en SQLite-database og AsyncStorage på din iPhone.
Hverken JacArrow eller nogen tredjepart har adgang til disse data.

### iCloud (kun når iCloud Drive er aktiveret)
JacArrow planlægger at bruge iCloud Key-Value Storage til ét bestemt formål:
at huske, om du allerede har startet prøveperioden. Dette synkroniseres
via din iCloud-konto for at forhindre, at afinstallation + geninstallation
giver en ny gratis prøveperiode.

- Apple er databehandler (vores aftale er underlagt deres standardvilkår)
- De gemte værdier er **kun**: dato for prøveperiodens start og en «prøve-brugt»-status
- Funktionen aktiveres, når vi lancerer Pro-modellen (Fase 4b)

Hvis du har deaktiveret iCloud Drive, eller deaktiveret iCloud Drive specifikt
for JacArrow, bruges iCloud ikke.

---

## Tredjeparter

### Apple App Store
Alle in-app-køb håndteres af Apple. Vi modtager aldrig kortoplysninger,
adresser eller andre betalingsdetaljer. Apples
[privatlivspolitik](https://www.apple.com/dk/legal/privacy/) gælder for
købsflowet.

### Apple Push Notification Service (APNS)
JacArrow sender lokale notifikationer (PR opnået, prøveperiode udløber,
målpåmindelser). For at levere dem registrerer iOS et anonymt enheds-token
hos Apple. Vi har ingen servere, der sender push-beskeder — alle notifikationer
genereres lokalt på din enhed baseret på app-tilstand.

### RevenueCat (kun efter Pro-køb)
Når du køber JacArrow Pro, registrerer RevenueCat din kvittering og et
anonymt `appUserId` (UUID genereret på din enhed). Dette er nødvendigt for,
at appen kan verificere dit køb ved senere brug og ved «Gendan
køb». RevenueCats
[privatlivspolitik](https://www.revenuecat.com/privacy) gælder. Vi sender aldrig
dit navn, e-mail eller andre personoplysninger.

### Apple Analytics / nedbrudsrapporter
Hvis du har aktiveret «Del app-analyse» i iOS-indstillingerne, sender Apple
anonyme aggregerede data om brug og nedbrud til udvikleren.
JacArrow bruger dette til fejlrettelse og ydeevneoptimering. Du kan
deaktivere dette via:
**iOS-indstillinger → Anonymitet og sikkerhed → Analyse og forbedringer**.

### Sentry (kun hvis du har aktiveret nedbrudsrapporter)
Sentry er en fejlovervågningstjeneste, der hjælper os med at identificere og rette
fejl i JacArrow. Sentry modtager kun data, hvis du har givet
**udtrykkeligt samtykke** via **Indstillinger → Privatliv → Nedbrudsrapporter**
(kontakten er som standard SLÅET FRA).

Når den er slået til, sendes følgende til Sentrys EU-servere (Tyskland):
- Nedbruds-stack traces (filnavne, linjenumre, exception-typer)
- Enhedsmodel og iOS-version
- App-version og build-nummer

Vi sender **ikke**:
- Personlige oplysninger (intet navn, ingen e-mail, intet bruger-ID knyttet til identitet)
- Ydelses-traces eller transaktioner (`tracesSampleRate: 0`)
- IP-adresser (`sendDefaultPii: false`)

Du kan deaktivere nedbrudsrapporter når som helst via den samme kontakt. Når den er
deaktiveret, **initialiseres Sentry ikke**, og der foretages ingen netværksanmodninger.
Sentrys [privatlivspolitik](https://sentry.io/privacy/) gælder for modtagne data.

---

## Det vi IKKE indsamler

- Ingen brugerkonto, e-mailadresse eller adgangskode
- Ingen GPS- eller positionsdata
- Ingen adgang til kontakter, kalender, kamera eller mikrofon
- Ingen tredjeparts-trackere (Firebase, Google Analytics, Facebook Pixel osv.)
- Ingen reklame-identifikatorer (IDFA)
- Ingen video-tracking eller enheds-fingeraftryk

---

## Dine rettigheder (GDPR)

Du har følgende rettigheder under databeskyttelsesforordningen:

**Ret til indsigt (Art. 15):** Alle dine data er gemt lokalt på din enhed.
Du har fuld indsigt via:
- Indstillinger → Mine pas (alle historiske runder)
- Indstillinger → Mine mål (alle aktive og arkiverede mål)
- Indstillinger → Buer / Pilset / Baner (udstyrsstyring)

**Ret til dataportabilitet (Art. 20):** Brug
**Indstillinger → Eksportér mine data** for at downloade alle dine data som
en JSON-fil. Filen kan deles via iOS' delemenu til e-mail, AirDrop, Filer osv.
Dette er din komplette skydehistorik i et standardformat.

**Ret til sletning (Art. 17):**
- *Slet enkelt pas:* stryg passet på hjemmeskærmen → Slet
- *Slet alle data:* afinstallér JacArrow — iOS sletter automatisk hele
  SQLite-databasen og AsyncStorage. RevenueCat-kvittering (hvis du har
  købt Pro) opbevares af Apple og RevenueCat til refusion og support.

**Ret til begrænsning og indsigelse (Art. 18–21):** JacArrow træffer
ingen automatiserede beslutninger om dig. Smart Insights-motoren analyserer kun
dine egne træningsdata lokalt på din enhed og præsenterer
observationer — den træffer ingen beslutninger på dine vegne.

**Ret til at trække samtykke tilbage (Art. 7):** Apple Analytics-opt-in styres
via iOS-indstillingerne. RevenueCat-data slettes, når du sletter dit Apple-ID.

---

## Ændringer

Vi opdaterer denne politik, når der sker væsentlige ændringer i, hvordan vi
behandler data. Ændringer kommunikeres via:
1. Datoen «Sidst opdateret» øverst på denne side
2. In-app-banner ved første åbning efter opdatering, hvis ændringen er væsentlig
   (fx nye tredjeparter, ny dataindsamling)

---

## Klager

Hvis du mener, at vi behandler dine personoplysninger i strid med GDPR, har du
ret til at klage til din nationale tilsynsmyndighed:

- **Danmark:** [Datatilsynet](https://www.datatilsynet.dk/)
- **EU/EØS:** find din myndighed på
  [edpb.europa.eu](https://www.edpb.europa.eu/about-edpb/about-edpb/members_en)

Vi opfordrer dig til at kontakte os først på galge.vender.0a@icloud.com — vi tager
alle privatlivshenvendelser alvorligt.
