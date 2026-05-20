# Tuki — ArrowTrack

**Viimeksi päivitetty:** 2026-05-20
**Kattaa version:** v1.0+
**Yhteystiedot:** galge.vender.0a@icloud.com

---

## Pika-apu

### Miten rekisteröin sarjan?

1. Avaa ArrowTrack → napauta **Uusi harjoitus** Koti-välilehdellä
2. Valitse paikka, taulu ja kierrosmuoto → napauta **Aloita harjoitus**
3. **Napauta taulua** sijoittaaksesi jokaisen nuolen — käytä pinch-zoomia ja tarkkuussuurennuslasia tarkkuuden varmistamiseksi
4. Napauta **Tallenna sarja**, kun kaikki nuolet on sijoitettu
5. Toista jokaiselle sarjalle, kunnes kierros on valmis

### Mitä eroa on X:llä ja 10:llä?

X-rengas on sisin rengas ja sen arvo on 10 pistettä — sama kuin 10-renkaan. ArrowTrack seuraa X:ää erikseen, koska X:ää käytetään tasapelin ratkaisuun kilpailuissa. Napauta «X»-painiketta, kun nuoli osuu X-renkaaseen score-pad-tilassa.

### Miten korjaan väärin sijoitetun nuolen?

1. Pitkä painallus nuolta taululla → tarkkuussuurennuslasi aktivoituu
2. Vedä nuoli uuteen sijaintiin → vapauta
3. TAI napauta nuolta valitaksesi sen → napauta **Poista** poistaaksesi sen

Score-pad-tilassa: napauta score-padin nuolimerkkiä ja valitse uusi arvo.

### Mitä on jälkirekisteröinti (📋-kuvake)?

📋-kuvake merkitsee harjoituksia, jotka on syötetty käsin score-padilla, ei rekisteröity taululle koordinaateilla. Osumakartta, konstellaatio ja hajonta-analyysi eivät ole käytettävissä jälkirekisteröityihin harjoituksiin — vain pistesummiin.

### Miten ostan Pron?

1. Napauta mitä tahansa Pro-lukittua ominaisuutta (esim. Pro-merkillä lukittu teema)
2. Paywall ilmestyy painikkeella **Osta Pro (299 NOK)**
3. Applen vakio-ostodialogi ilmestyy → vahvista Face ID:llä / pääsykoodilla
4. Pro aktivoituu välittömästi — kaikki ominaisuudet avautuvat

**Hinta:** 299 NOK kertaosto, elinikäinen. Ei tilausta, ei toistuvia veloituksia.

### Miten palautan ostot uudella iPhonella?

1. Lataa ArrowTrack uudelle iPhonelle (ilmaisversio)
2. Kirjaudu sisään samalla Apple-ID:llä, jolla ostit Pron
3. Avaa ArrowTrack → **Asetukset → Lisenssi → Palauta ostot**
4. Pro aktivoituu uudelleen automaattisesti

Jos olet vaihtanut Apple-ID:tä: ota yhteyttä galge.vender.0a@icloud.com, niin autamme.

### Miten vien tietoni?

**Asetukset → Tietoja sovelluksesta → Vie tietoni** → iOS:n jakovalikko avautuu. Valitse AirDrop, Mail, Tiedostot tai minne haluat lähettää JSON-tiedoston.

JSON sisältää kaikki harjoitukset, kierrokset, nuolet, tavoitteet, jousiasetelmat ja asetukset — täysi siirrettävyys GDPR Art. 20:n mukaisesti.

### Miten poistan kaikki tietoni?

Poista ArrowTrack → iOS poistaa automaattisesti koko SQLite-tietokannan ja kaikki asetukset. Laitteelle ei jää jäännöstietoja.

Jos olet ostanut Pron: kuitti säilyy Applella (palautus- ja tukitarpeisiin). Poisto ei vaikuta tuleviin uudelleenasennuksiin — Pro aktivoituu automaattisesti Palauta ostot -toiminnolla.

### Mitä kierrosmuotoja tuetaan?

- **WA 720** (ulkona, 6 sarjaa × 12 nuolta = 72 nuolta)
- **WA 18 m sisällä** (10 sarjaa × 3 nuolta)
- **WA 1440** (4 peräkkäistä matkaa)
- **Vegas Shoot** (10 sarjaa × 3 nuolta sisällä 18 m)
- **AGB Portsmouth** (10 sarjaa × 3 nuolta sisällä 20 yd)
- **NFAA Indoor** (12 sarjaa × 5 nuolta sisällä 20 yd)
- **Vapaa harjoittelu** (ei muotorajoituksia)

Kaikki muodot sisältävät virallisen WA Book 3 -yhteensopivuuden: viivasääntö, erillinen X-seuranta, oikeat renkaiden säteet.

### Mitä tauluja tuetaan?

- **WA 122 cm 10-rengas** (ulkostandardi)
- **WA 80 cm 10-rengas** (ulkona pitkä matka)
- **WA 40 cm 10-rengas** (sisällä, yksittäinen spot)
- **WA 40 cm Vegas 3-spot kolmiomainen** (sisäkilpailu)
- **WA 40 cm Vegas 3-spot pystysuora** (sisävaihtoehto)
- **AGB Portsmouth 60 cm 10-rengas** (sisällä UK)
- **NFAA sisällä yksittäinen spot sininen 40 cm** (USA)
- **NFAA sisällä 5-spot sininen 40 cm** (USA-kilpailu)

---

## Tekniset ongelmat

### Sovellus kaatuu käynnistyksessä

1. Sammuta iPhone ja käynnistä uudelleen
2. Jos ongelma jatkuu: poista ja asenna ArrowTrack uudelleen (ostotietoja EI menetetä — kuitti säilyy Applella)
3. Lähetä kaatumisloki osoitteeseen galge.vender.0a@icloud.com: **Asetukset → Tietosuoja ja turvallisuus → Analytiikka ja parannukset → Analyysitiedot** → etsi ArrowTrack-loki → jaa kanssamme

Jos olet valinnut jakaa analytiikan kehittäjän kanssa iOS:n kautta, kaatumislokit lähetetään meille automaattisesti.

### Pistetiedot katosivat päivityksen jälkeen

ArrowTrack tallentaa kaiken paikallisesti SQLiteen. Päivitykset siirtävät tietokantaa vain eteenpäin — vanhat tiedot muunnetaan uuteen muotoon, niitä ei koskaan poisteta.

Jos koet tietojen katoamista:
1. Varmista, että olet kirjautunut samalla Apple-ID:llä
2. Tarkista **Asetukset → Tietoja sovelluksesta → Versionumero** — onko se viimeisin?
3. Lähetä meille kuvaus osoitteeseen galge.vender.0a@icloud.com

Meillä on tiukka sääntö, että julkaistut migraatiot ovat muuttumattomia — tietojen katoamista päivityksistä ei pitäisi koskaan tapahtua. Jos näin käy, meillä on bugi ja haluamme kuulla siitä.

### Pinch-zoom ei toimi taululla

1. Kokeile kahdella sormella, älä yhdellä
2. Tarkista, ettei sinulla ole «Vähennä liikettä» päällä **iOS-asetukset → Käytettävyys → Liike** — se voi rajoittaa eleitä joissakin sovelluksissa
3. Sulje sovellus kokonaan (pyyhkäise ylöspäin alhaalta, pyyhkäise ArrowTrack ylöspäin) ja avaa uudelleen

### Konstellaationäkymä tärisee vetäessä

Tämä oli bugi versioissa v0.28.2 ja aiemmissa — korjattu versiossa v0.28.3. Päivitä sovellus uusimpaan versioon App Storessa.

---

## Palaute ja pyynnöt

### Ehdota uutta ominaisuutta

Lähetä sähköposti osoitteeseen galge.vender.0a@icloud.com:
- **Mitä** haluat (lyhyt kuvaus)
- **Miksi** (mitä se parantaisi harjoittelussasi?)
- **Kuinka usein** käyttäisit sitä (päivittäin / per harjoitus / harvemmin)

Luemme jokaisen pyynnön ja julkaisemme priorisoidut ominaisuudet sovelluksen «Mitä uutta» -syötteessä.

### Ilmoita bugista

Lähetä sähköposti osoitteeseen galge.vender.0a@icloud.com:
- **Mikä meni pieleen** (niin yksityiskohtaisesti kuin pystyt)
- **Mitä odotit tapahtuvan**
- **Vaihe vaiheelta** toistettavaksi
- **iOS-versio** ja **iPhone-malli** (Asetukset → Yleiset → Tietoja)
- **ArrowTrackin versio** (Asetukset → Tietoja sovelluksesta)
- Kuvakaappaus tarvittaessa

### Yleistä
Vastaamme kaikkiin yhteydenottoihin 3 arkipäivän kuluessa. Kiireelliset ongelmat (kaatumiset, jotka estävät ampumisen) priorisoidaan korkeammalle.

---

## GDPR ja tietosuoja

Täydellinen tietosuojakäytäntö: [Tietosuoja](https://mjacobsen71.github.io/arrowtrack-legal/privacy-fi)

Tietojesi viemiseen, harjoituksen poistamiseen tai muiden GDPR-oikeuksien käyttämiseen: katso Tietosuojakäytäntö.

Tietosuojaa koskevat valitukset: ota yhteyttä meihin **ensin** osoitteessa galge.vender.0a@icloud.com. Jos emme pysty ratkaisemaan asiaa, voit valittaa kansalliselle tietosuojaviranomaisellesi. Suomessa: [Tietosuojavaltuutetun toimisto](https://tietosuoja.fi/).

---

## Tietoa ArrowTrackista

**Kehittäjä:** Morten Jacobsen, Norja
**Kotisivu:** [mjacobsen71.github.io/arrowtrack-legal](https://mjacobsen71.github.io/arrowtrack-legal)
**Tietosuojakäytäntö:** [Tietosuoja](https://mjacobsen71.github.io/arrowtrack-legal/privacy-fi)
**Lisenssit (avoin lähdekoodi):** katso Asetukset → Tietoja sovelluksesta → Lisenssit sovelluksessa

ArrowTrack on yhden kehittäjän projekti, joka on rakennettu jousiampujille kaikilla tasoilla — ensimmäisestä nuolesta sadanteen kilpailuun. WA Book 3 -yhteensopiva pisteytys on mukana ensimmäisestä päivästä, valmiina kun haluat sen. Rakennettu React Nativella + Expolla + TypeScriptillä + SQLitella. Ei backendia, ei pilveä, ei seurantaa.

Kiitos, että käytät sovellusta. 🏹
