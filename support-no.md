# Support — JacArrow

**Sist oppdatert:** 2026-05-20
**Versjon dekket:** v1.0+
**Kontakt:** galge.vender.0a@icloud.com

---

## Hurtig hjelp

### Hvordan registrerer jeg en serie?

1. Åpne JacArrow → trykk **Ny økt** på Hjem-fanen
2. Velg sted, skive, og runde-format → trykk **Start økt**
3. **Trykk på skiva** for å plassere hver pil — bruk pinch-zoom og presisjonslupe for nøyaktighet
4. Trykk **Lagre serie** når alle piler er plassert
5. Gjenta for hver serie til runden er ferdig

### Hva er forskjellen på X og 10?

X-ringen er den innerste ringen og scorer 10 poeng — akkurat som 10-ringen. JacArrow sporer X separat fordi X brukes som tiebreaker i konkurranser. Tap «X»-knappen når en pil treffer X-ringen i score-pad-modus.

### Hvordan rediger jeg en feil-registrert pil?

1. Lang-trykk på pilen på skiva → presisjons-lupen aktiveres
2. Dra pilen til ny posisjon → slipp
3. ELLER trykk på pilen for å velge → trykk **Slett**-knappen for å fjerne den

I etterregistrering-modus: trykk på pil-merket i score-pad og velg ny verdi.

### Hva er etterregistrering (📋-ikonet)?

📋-ikonet markerer økter som er lagt inn manuelt med score-pad'en, ikke registrert på skiva med koordinater. Treffbilde, konstellasjon og spredningsanalyse er ikke tilgjengelig for etterregistrerte økter — kun score-totalen.

### Hvordan kjøper jeg Pro?

1. Trykk på en Pro-låst funksjon (eks. et tema låst med Pro-merke)
2. Paywall vises med **Kjøp Pro (kr 299)**-knapp
3. Apple's standard kjøps-modal vises → bekreft med Face ID / passord
4. Pro aktiveres umiddelbart — alle features låses opp

**Pris:** Kr 299 engangskjøp, lifetime. Ingen abonnement, ingen tilbakevendende belastninger.

### Hvordan gjenoppretter jeg kjøp på ny iPhone?

1. Last ned JacArrow på den nye iPhone (gratis-versjonen)
2. Logg inn med samme Apple-ID du brukte til å kjøpe Pro
3. Åpne JacArrow → **Innstillinger → Lisens → Gjenopprett kjøp**
4. Pro reaktiveres automatisk

Hvis du har byttet Apple-ID: kontakt galge.vender.0a@icloud.com så hjelper vi deg.

### Hvordan eksporterer jeg data?

**Innstillinger → Om appen → Eksporter mine data** → iOS' delings-meny dukker opp. Velg AirDrop, Mail, Filer, eller hvor du vil sende JSON-filen.

JSON-en inneholder alle sesjoner, runder, piler, mål, bue-oppsett, og innstillinger — komplett portabilitet under GDPR Art. 20.

### Hvordan sletter jeg alle data?

Avinstaller JacArrow → iOS fjerner automatisk hele SQLite-databasen og alle innstillinger. Ingen rest-data forblir på enheten.

Hvis du har kjøpt Pro: kvitteringen forblir hos Apple (for refund- og support-behov). Avinstallasjon påvirker ikke fremtidige re-installasjoner — Pro reaktiveres automatisk ved gjenopprett.

### Hvilke runde-formater støttes?

- **WA 720** (utendørs, 6 endinger × 12 piler = 72 piler)
- **WA 18 m innendørs** (10 endinger × 3 piler)
- **WA 1440** (4 sekvensielle distanser)
- **Vegas Shoot** (10 endinger × 3 piler indoor 18 m)
- **AGB Portsmouth** (10 endinger × 3 piler indoor 20 yd)
- **NFAA Indoor** (12 endinger × 5 piler indoor 20 yd)
- **Fri trening** (ingen format-grenser)

Alle formater inkluderer offisiell WA Book 3-compliance: line-breaking-regel, separat X-tracking, korrekte ring-radier.

### Hvilke skive-typer støttes?

- **WA 122 cm 10-ring** (utendørs standard)
- **WA 80 cm 10-ring** (utendørs lang distanse)
- **WA 40 cm 10-ring** (innendørs, enkelt-spot)
- **WA 40 cm Vegas 3-spot triangulær** (innendørs konkurranse)
- **WA 40 cm Vegas 3-spot vertikal** (innendørs alternativ)
- **AGB Portsmouth 60 cm 10-ring** (innendørs UK)
- **NFAA innendørs enkelt-spot blå 40 cm** (USA)
- **NFAA innendørs 5-spot blå 40 cm** (USA konkurranse)

---

## Tekniske problemer

### Appen krasjer ved oppstart

1. Slå av iPhone og start på nytt
2. Hvis fortsatt problem: avinstaller og reinstaller JacArrow (kjøps-data tapes IKKE — kvittering forblir hos Apple)
3. Send krasj-logg til galge.vender.0a@icloud.com: **Innstillinger → Personvern og sikkerhet → Analytics og forbedringer → Analytics Data** → finn JacArrow-logg → del med oss

Hvis du har valgt å dele analytics med utvikleren via iOS, sendes krasj-logger automatisk til oss.

### Score-data forsvant etter oppdatering

JacArrow lagrer alt lokalt i SQLite. Oppdateringer migrerer databasen forward-only — gamle data konverteres til nytt format, aldri slettes.

Hvis du opplever data-tap:
1. Verifiser at du er logget inn med samme Apple-ID
2. Sjekk **Innstillinger → Om appen → Versjonsnummer** — er den oppdatert?
3. Send oss en beskrivelse på galge.vender.0a@icloud.com

Vi har en strikt regel om at publiserte migrations er immutable — data-tap fra oppdateringer skal aldri skje. Hvis det gjør det, har vi en bug og vi vil høre om det.

### Pinch-zoom virker ikke på skiva

1. Prøv med to fingre, ikke én
2. Sjekk at du ikke har «Redusert bevegelse» (Reduce Motion) skrudd på i **iOS Innstillinger → Tilgjengelighet → Bevegelse** — det kan begrense gestures i noen apper
3. Lukk appen helt (sveip opp fra bunnen, sveip JacArrow opp) og åpne på nytt

### Konstellasjons-visningen vibrerer ved drag

Dette var en bug i v0.28.2 og tidligere — fikset i v0.28.3. Oppdater appen til siste versjon i App Store.

---

## Tilbakemelding og forespørsler

### Foreslå nye features

Send en e-post til galge.vender.0a@icloud.com med:
- **Hva** du vil ha (kort beskrivelse)
- **Hvorfor** (hva ville det forbedre i din skytetrening?)
- **Hvor ofte** ville du brukt det (daglig / per økt / sjeldnere)

Vi leser hver eneste forespørsel og publiserer prioriterte features i appens «Hva er nytt»-strøm.

### Rapporter bug

Send en e-post til galge.vender.0a@icloud.com med:
- **Hva som gikk galt** (skriv så detaljert du klarer)
- **Hva du forventet å skje**
- **Steg-for-steg** for hvordan reprodusere
- **iOS-versjon** og **iPhone-modell** (Innstillinger → Generelt → Om)
- **JacArrow-versjon** (Innstillinger → Om appen)
- Skjermbilde hvis aktuelt

### Generelt
Vi svarer på alle henvendelser innen 3 virkedager. Akutte problemer (krasj som hindrer deg fra å skyte) prioriteres høyere.

---

## GDPR og personvern

For full personvernerklæring: [Personvern](https://mjacobsen71.github.io/jacarrow-legal/privacy-no)

For å eksportere dataene dine, slette en sesjon, eller utøve andre GDPR-rettigheter: se Personvernerklæringen.

Klager om personvern: kontakt oss på galge.vender.0a@icloud.com **først**. Hvis vi ikke løser saken, kan du klage til [Datatilsynet](https://www.datatilsynet.no/).

---

## Om JacArrow

**Utvikler:** Morten Jacobsen, Norge
**Hjemmeside:** [mjacobsen71.github.io/jacarrow-legal](https://mjacobsen71.github.io/jacarrow-legal)
**Privacy Policy:** [Personvern](https://mjacobsen71.github.io/jacarrow-legal/privacy-no)
**Lisenser (open source):** Se Innstillinger → Om appen → Lisenser i appen

JacArrow er et solo-utvikler-prosjekt bygget for bueskyttere på alle nivåer — fra første pil til hundrede stevne. WA Book 3-kompatibel scoring er der fra dag én, klar når du vil ha den. Bygget med React Native + Expo + TypeScript + SQLite. Ingen backend, ingen sky, ingen sporing.

Takk for at du bruker appen. 🏹
