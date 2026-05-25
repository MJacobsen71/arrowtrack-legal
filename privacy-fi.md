# Tietosuojakäytäntö — JacArrow

**Viimeksi päivitetty:** 2026-05-25
**Rekisterinpitäjä:** Morten Jacobsen, Norja
**Yhteystiedot:** galge.vender.0a@icloud.com

---

## Lyhyt versio

JacArrow tallentaa **kaikki tietosi paikallisesti laitteellesi**. Meillä ei ole
palvelimia, jotka vastaanottaisivat ammuntojasi, harjoituksiasi tai tavoitteitasi. Kun
poistat sovelluksen, kaikki tiedot katoavat.

Ainoat kolmannet osapuolet, jotka saavat tietoja, ovat:
- **Apple** — käsittelee App Store -ostot ja ilmoitukset
- **RevenueCat** (Pro-oston jälkeen) — varmistaa ostosi
- **Sentry** (vain jos otat kaatumisraportit käyttöön) — vastaanottaa anonyymejä kaatumistietoja, jotta voimme korjata virheitä

Sinulla on täydet GDPR-oikeudet pääsyyn, poistoon ja tietojen siirrettävyyteen.

---

## Mitä tallennamme

### Laitteellasi (paikallisesti, ei poistu puhelimesta)
- **Ammuntatiedot:** harjoitukset, kierrokset, nuolten sijoittelut, pisteet, tunnisteet, tavoitteet, jouset ja nuolisetit
- **Asetukset:** valittu kieli, teema, ampumakäsi, kilpailuluokka, ilmoitusasetukset
- **Sovellushistoria:** coach-mark-tila (mitä vinkkejä olet nähnyt), tutoriaali-suoritettu-liput

Kaikki nämä tiedot tallennetaan SQLite-tietokantaan ja AsyncStorageen iPhonellesi.
Sen enempää JacArrowilla kuin millään kolmannella osapuolella ei ole pääsyä näihin tietoihin.

### iCloud (vain kun iCloud Drive on käytössä)
JacArrow aikoo käyttää iCloud Key-Value Storagea yhteen tarkkaan tarkoitukseen:
muistamaan, oletko aiemmin aloittanut kokeilujakson. Tämä synkronoituu
iCloud-tilisi kautta estääkseen sen, että poistaminen + uudelleenasennus
antaisi uuden ilmaisen kokeilujakson.

- Apple on tietojenkäsittelijä (sopimuksemme noudattaa heidän vakioehtojaan)
- Tallennetut arvot ovat **vain**: kokeilun aloituspäivä ja «kokeilu käytetty» -tila
- Tämä ominaisuus aktivoituu, kun lanseeraamme Pro-mallin (Vaihe 4b)

Jos olet poistanut iCloud Driven käytöstä tai poistanut iCloud Driven käytöstä erityisesti
JacArrowilta, iCloudia ei käytetä.

---

## Kolmannet osapuolet

### Apple App Store
Kaikki sovelluksen sisäiset ostot hoitaa Apple. Emme koskaan vastaanota korttitietoja,
osoitteita tai muita maksutietoja. Applen
[tietosuojakäytäntö](https://www.apple.com/fi/legal/privacy/) koskee
ostoprosessia.

### Apple Push Notification Service (APNS)
JacArrow lähettää paikallisia ilmoituksia (PE saavutettu, kokeilujakson päättyminen,
tavoitemuistutukset). Niiden toimittamiseksi iOS rekisteröi anonyymin laitetunnuksen
Applelle. Meillä ei ole palvelimia, jotka lähettäisivät push-viestejä — kaikki ilmoitukset
luodaan paikallisesti laitteellasi sovelluksen tilan perusteella.

### RevenueCat (vain Pro-oston jälkeen)
Kun ostat JacArrow Pron, RevenueCat tallentaa kuittisi ja
anonyymin `appUserId`:n (laitteellasi luotu UUID). Tämä on tarpeen
sovelluksen ostosi varmistamiseen myöhemmässä käytössä ja «Palauta
ostot» -toiminnossa. RevenueCatin
[tietosuojakäytäntö](https://www.revenuecat.com/privacy) koskee tätä. Emme koskaan lähetä
nimeäsi, sähköpostiosoitettasi tai muita henkilötietoja.

### Apple Analytics / kaatumisraportit
Jos olet ottanut käyttöön «Jaa sovelluksen analyysit» iOS-asetuksissa, Apple lähettää
anonyymejä koostettuja tietoja käytöstä ja kaatumisista kehittäjälle.
JacArrow käyttää tätä virheenkorjaukseen ja suorituskyvyn optimointiin. Voit
poistaa tämän käytöstä:
**iOS-asetukset → Tietosuoja ja turvallisuus → Analytiikka ja parannukset**.

### Sentry (vain jos olet ottanut kaatumisraportit käyttöön)
Sentry on virheidenseurantapalvelu, joka auttaa meitä tunnistamaan ja korjaamaan
virheitä JacArrowissa. Sentry vastaanottaa tietoja vain, jos olet antanut siihen
**nimenomaisen suostumuksen** kohdasta **Asetukset → Tietosuoja → Kaatumisraportit**
(kytkin on oletuksena POIS päältä).

Kun ominaisuus on käytössä, Sentryn EU-palvelimille (Saksa) lähetetään seuraavat:
- Kaatumisten pinojäljet (tiedostonimet, rivinumerot, poikkeustyypit)
- Laitemalli ja iOS-versio
- Sovellusversio ja build-numero

Emme lähetä:
- Henkilökohtaisia tietoja (ei nimeä, ei sähköpostia, ei identiteettiin liitettyä käyttäjätunnusta)
- Suorituskykyjälkiä tai tapahtumia (`tracesSampleRate: 0`)
- IP-osoitteita (`sendDefaultPii: false`)

Voit poistaa kaatumisraportit käytöstä milloin tahansa samalla kytkimellä. Kun ominaisuus on
poissa käytöstä, Sentryä **ei alusteta** eikä verkkopyyntöjä tehdä.
Sentryn [tietosuojakäytäntö](https://sentry.io/privacy/) koskee vastaanotettuja tietoja.

---

## Mitä EMME kerää

- Ei käyttäjätiliä, sähköpostiosoitetta tai salasanaa
- Ei GPS- tai sijaintitietoja
- Ei pääsyä yhteystietoihin, kalenteriin, kameraan tai mikrofoniin
- Ei kolmansien osapuolten seurantoja (Firebase, Google Analytics, Facebook Pixel jne.)
- Ei mainostunnisteita (IDFA)
- Ei video-seurantaa eikä laitteen sormenjälkeä

---

## Oikeutesi (GDPR)

Sinulla on seuraavat oikeudet yleisen tietosuoja-asetuksen mukaan:

**Oikeus tutustua tietoihin (Art. 15):** Kaikki tietosi on tallennettu paikallisesti laitteellesi.
Sinulla on täysi näkyvyys:
- Asetukset → Omat harjoitukset (kaikki historialliset kierrokset)
- Asetukset → Omat tavoitteet (kaikki aktiiviset ja arkistoidut tavoitteet)
- Asetukset → Jouset / Nuolisetit / Ammuntapaikat (varustehallinta)

**Oikeus tietojen siirrettävyyteen (Art. 20):** Käytä
**Asetukset → Vie tietoni** ladataksesi kaikki tietosi JSON-tiedostona. Tiedosto
voidaan jakaa iOS-jakovalikon kautta sähköpostiin, AirDropiin, Tiedostoihin jne.
Tämä on täydellinen ammuntahistoriasi standardimuodossa.

**Oikeus tietojen poistamiseen (Art. 17):**
- *Poista yksittäinen harjoitus:* pyyhkäise harjoitusta aloitusnäytössä → Poista
- *Poista kaikki tiedot:* poista JacArrow — iOS poistaa automaattisesti koko
  SQLite-tietokannan ja AsyncStoragen. RevenueCat-kuitti (jos olet
  ostanut Pron) säilyy Applella ja RevenueCatilla palautus- ja tukitarpeisiin.

**Oikeus käsittelyn rajoittamiseen ja vastustamiseen (Art. 18–21):** JacArrow ei tee
mitään automatisoituja päätöksiä sinusta. Smart Insights -moottori analysoi vain
omia harjoitustietojasi paikallisesti laitteellasi ja esittää
havaintoja — se ei tee päätöksiä puolestasi.

**Oikeus peruuttaa suostumus (Art. 7):** Apple Analyticsin opt-in hallitaan
iOS-asetuksissa. RevenueCat-tiedot poistetaan, kun poistat Apple-ID:si.

---

## Muutokset

Päivitämme tätä käytäntöä, kun tapahtuu merkittäviä muutoksia siinä, miten käsittelemme
tietoja. Muutoksista viestitään:
1. Sivun yläosan «Viimeksi päivitetty» -päivämäärän kautta
2. Sovelluksensisäisen bannerin kautta päivityksen jälkeisellä ensimmäisellä käynnistyksellä, jos muutos on merkittävä
   (esim. uudet kolmannet osapuolet, uusi tiedonkeruu)

---

## Valitukset

Jos uskot, että käsittelemme henkilötietojasi GDPR:n vastaisesti, sinulla on
oikeus tehdä valitus kansalliselle tietosuojaviranomaisellesi:

- **Suomi:** [Tietosuojavaltuutetun toimisto](https://tietosuoja.fi/)
- **EU/ETA:** löydä viranomaisesi osoitteesta
  [edpb.europa.eu](https://www.edpb.europa.eu/about-edpb/about-edpb/members_en)

Suosittelemme ottamaan yhteyttä meihin ensin osoitteessa galge.vender.0a@icloud.com — otamme
kaikki tietosuojakyselyt vakavasti.
