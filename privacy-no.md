# Personvernerklæring — ArrowTrack

**Sist oppdatert:** 2026-05-15
**Behandlingsansvarlig:** Morten Jacobsen, Norge
**Kontakt:** galge.vender.0a@icloud.com

---

## Kort versjon

ArrowTrack lagrer **all dine data lokalt på enheten din**. Vi har ingen
servere som mottar dine skytinger, økter eller målsetting. Når du
avinstallerer appen forsvinner all data.

De eneste tredjepartene som mottar informasjon er:
- **Apple** — håndterer App Store-kjøp og varsler
- **RevenueCat** (etter du har kjøpt Pro) — verifiserer kjøpet

Du har full rett til innsyn, sletting og dataportabilitet under GDPR.

---

## Hva vi lagrer

### På enheten din (lokalt, forlater aldri telefonen)
- **Skytte-data:** økter, runder, pile-plasseringer, score, tagger, mål, buer og pilesett
- **Innstillinger:** valgt språk, tema, dominant hånd, konkurranseklasse, varslings-toggles
- **Apphistorikk:** coach-mark-status (hvilke tips du har sett), tutorial-fullført-flagg

All denne data er lagret i SQLite-database og AsyncStorage på din iPhone. Hverken
ArrowTrack eller noen tredjepart har tilgang til denne dataen.

### iCloud (kun ved aktivert iCloud Drive)
ArrowTrack planlegger å bruke iCloud Key-Value Storage til ett spesifikt formål:
huske om du har startet prøveperioden tidligere. Dette synkroniseres via din
iCloud-konto for å hindre at avinstall + reinstall gir en ny gratis prøveperiode.

- Apple er databehandler (vår avtale er underlagt deres standardvilkår)
- Verdiene som lagres er **kun**: dato for prøveperiode-start, og en
  «prøveperiode-brukt»-status
- Funksjonen aktiveres når vi launcher Pro-modellen (Phase 4b)

Hvis du har deaktivert iCloud Drive, eller deaktiverer iCloud Drive for
ArrowTrack spesifikt, brukes ikke iCloud.

---

## Tredjeparter

### Apple App Store
Alle in-app-kjøp håndteres av Apple. Vi mottar aldri kortinformasjon,
adresser, eller andre betalings-detaljer. Apples
[personvernerklæring](https://www.apple.com/no/legal/privacy/) gjelder for
kjøps-flyten.

### Apple Push Notification Service (APNS)
ArrowTrack sender lokale varsler (PR-oppnådd, prøveperiode-utløp, påminnelser
om mål). For å levere disse registrerer iOS et anonymt enhets-token med Apple.
Vi har ingen servere som sender push-meldinger — alle varsler genereres
lokalt på enheten din basert på app-tilstand.

### RevenueCat (kun etter Pro-kjøp)
Når du kjøper ArrowTrack Pro registrerer RevenueCat ditt kvittering og en
anonym `appUserId` (UUID generert på enheten din). Dette er nødvendig for at
appen skal kunne verifisere ditt kjøp ved senere bruk og ved «Gjenopprett
kjøp». RevenueCats [personvernerklæring](https://www.revenuecat.com/privacy)
gjelder. Vi sender aldri ditt navn, e-post, eller andre personopplysninger.

### Apple Analytics / Crash Reports
Hvis du har aktivert «Del app-analyse» i iOS-innstillinger sender Apple
anonyme aggregat-data om bruk og krasj til utvikleren. ArrowTrack bruker dette
til feilretting og ytelses-optimering. Du kan deaktivere dette via:
**iOS Innstillinger → Personvern og sikkerhet → Analyse og forbedringer**.

---

## Det vi IKKE samler

- Ingen brukerkonto, e-postadresse, eller passord
- Ingen GPS- eller lokasjons-data
- Ingen tilgang til kontakter, kalender, kamera eller mikrofon
- Ingen tredjeparts trackers (Firebase, Google Analytics, Facebook Pixel, osv.)
- Ingen reklame-identifikatorer (IDFA)
- Ingen videooppfølging eller fingerprinting

---

## Dine rettigheter (GDPR)

Du har følgende rettigheter under personvernforordningen:

**Innsyn (Art. 15):** All din data ligger lokalt på enheten. Du har full
innsikt via:
- Innstillinger → Mine økter (alle historiske runder)
- Innstillinger → Mine mål (alle aktive og arkiverte mål)
- Innstillinger → Buer / Pilesett / Lokasjoner (utstyrshåndtering)

**Dataportabilitet (Art. 20):** Bruk
**Innstillinger → Eksporter mine data** for å laste ned all din data som
JSON-fil. Filen kan deles via iOS share-sheet til e-post, AirDrop, Filer,
osv. Dette er din komplette skytte-historikk i et standard format.

**Sletting (Art. 17):**
- *Slett enkelt-økt:* sveip økten på hjem-skjermen → Slett
- *Slett alle data:* avinstaller ArrowTrack — iOS sletter automatisk all
  SQLite-database og AsyncStorage. RevenueCat-kvittering (hvis du har kjøpt
  Pro) beholdes hos Apple og RevenueCat for refund- og support-formål.

**Begrensning og innsigelse (Art. 18–21):** ArrowTrack utfører ingen
automatiserte beslutninger om deg. Smart innsikt-motoren analyserer kun din
egen treningsdata lokalt på enheten og presenterer observasjoner — den tar
ingen beslutninger på dine vegne.

**Trekk samtykke tilbake (Art. 7):** Apple Analytics opt-in styres via
iOS Innstillinger. RevenueCat-data slettes ved sletting av Apple-ID.

---

## Endringer

Vi vil oppdatere denne erklæringen ved vesentlige endringer i hvordan vi
behandler data. Endringer kommuniseres via:
1. «Sist oppdatert»-dato på toppen av denne siden
2. In-app-banner ved første åpning etter oppdatering hvis endringen er
   vesentlig (eks. nye tredjeparter, ny datainnsamling)

---

## Klage

Hvis du mener vi behandler dine personopplysninger i strid med GDPR har du
rett til å klage til [Datatilsynet](https://www.datatilsynet.no/). Du
oppfordres til å kontakte oss først på galge.vender.0a@icloud.com — vi tar alle
henvendelser om personvern på alvor.
