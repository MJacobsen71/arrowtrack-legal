# Datenschutzerklärung — JacArrow

**Zuletzt aktualisiert:** 2026-05-25
**Verantwortlicher:** Morten Jacobsen, Norwegen
**Kontakt:** galge.vender.0a@icloud.com

---

## Kurzfassung

JacArrow speichert **alle deine Daten lokal auf deinem Gerät**. Wir haben keine
Server, die deine Schüsse, Trainingseinheiten oder Ziele empfangen. Wenn du
die App deinstallierst, sind alle Daten weg.

Die einzigen Dritten, die Informationen erhalten, sind:
- **Apple** — wickelt App-Store-Käufe und Benachrichtigungen ab
- **RevenueCat** (nachdem du Pro gekauft hast) — überprüft deinen Kauf
- **Sentry** (nur wenn du Absturzberichten zustimmst) — erhält anonyme Absturzdaten, damit wir Fehler beheben können

Du hast nach DSGVO volle Rechte auf Auskunft, Löschung und Datenübertragbarkeit.

---

## Was wir speichern

### Auf deinem Gerät (lokal, verlässt niemals das Smartphone)
- **Schießdaten:** Trainingseinheiten, Runden, Pfeilplatzierungen, Punktzahlen, Tags, Ziele, Bögen und Pfeilsätze
- **Einstellungen:** ausgewählte Sprache, Theme, Schießhand, Wettkampfklasse, Benachrichtigungsoptionen
- **App-Verlauf:** Coach-Mark-Status (welche Tipps du gesehen hast), Tutorial-Abschluss-Flags

Alle diese Daten werden in einer SQLite-Datenbank und in AsyncStorage auf deinem iPhone gespeichert.
Weder JacArrow noch ein Dritter hat Zugriff auf diese Daten.

### iCloud (nur bei aktiviertem iCloud Drive)
JacArrow plant, iCloud Key-Value Storage für einen spezifischen Zweck zu nutzen:
um sich zu merken, ob du den Testzeitraum bereits begonnen hast. Dies synchronisiert
sich über dein iCloud-Konto, um zu verhindern, dass Deinstallation + Neuinstallation
einen neuen kostenlosen Testzeitraum gewährt.

- Apple ist der Auftragsverarbeiter (unsere Vereinbarung unterliegt deren Standardbedingungen)
- Die gespeicherten Werte sind **nur**: das Trial-Startdatum und ein «Trial-genutzt»-Status
- Diese Funktion wird aktiviert, wenn wir das Pro-Modell starten (Phase 4b)

Wenn du iCloud Drive deaktiviert hast oder iCloud Drive speziell für
JacArrow deaktiviert hast, wird iCloud nicht genutzt.

---

## Dritte

### Apple App Store
Alle In-App-Käufe werden von Apple abgewickelt. Wir erhalten niemals Karteninformationen,
Adressen oder andere Zahlungsdetails. Apples
[Datenschutzrichtlinie](https://www.apple.com/legal/privacy/) gilt für
den Kaufvorgang.

### Apple Push Notification Service (APNS)
JacArrow sendet lokale Benachrichtigungen (PR erreicht, Ablauf des Testzeitraums,
Zielerinnerungen). Um diese zuzustellen, registriert iOS ein anonymes Geräte-Token
bei Apple. Wir haben keine Server, die Push-Nachrichten senden — alle Benachrichtigungen
werden lokal auf deinem Gerät basierend auf dem App-Zustand generiert.

### RevenueCat (nur nach Pro-Kauf)
Wenn du JacArrow Pro kaufst, zeichnet RevenueCat deine Quittung und eine
anonyme `appUserId` (eine auf deinem Gerät generierte UUID) auf. Dies ist notwendig,
damit die App deinen Kauf bei späterer Nutzung und beim «Käufe
wiederherstellen» überprüfen kann. RevenueCats
[Datenschutzrichtlinie](https://www.revenuecat.com/privacy) gilt. Wir senden niemals
deinen Namen, deine E-Mail oder andere personenbezogene Daten.

### Apple Analytics / Crash Reports
Wenn du «App-Analyse teilen» in den iOS-Einstellungen aktiviert hast, sendet Apple
anonyme aggregierte Daten über Nutzung und Abstürze an den Entwickler.
JacArrow nutzt dies für Fehlerbehebungen und Performance-Optimierung. Du kannst
dies deaktivieren über:
**iOS-Einstellungen → Datenschutz & Sicherheit → Analyse & Verbesserungen**.

### Sentry (nur wenn du Absturzberichte aktiviert hast)
Sentry ist ein Fehlerüberwachungsdienst, der uns hilft, Bugs in JacArrow zu
identifizieren und zu beheben. Sentry erhält nur dann Daten, wenn du dem
**ausdrücklich zugestimmt** hast über **Einstellungen → Datenschutz → Absturzberichte**
(der Schalter ist standardmäßig AUS).

Nach Opt-in wird Folgendes an Sentrys EU-Server (Deutschland) gesendet:
- Absturz-Stack-Traces (Dateinamen, Zeilennummern, Exception-Typen)
- Gerätemodell und iOS-Version
- App-Version und Build-Nummer

Wir senden **nicht**:
- Persönliche Informationen (kein Name, keine E-Mail, keine identitätsverknüpfte Nutzer-ID)
- Performance-Traces oder Transaktionen (`tracesSampleRate: 0`)
- IP-Adressen (`sendDefaultPii: false`)

Du kannst Absturzberichte jederzeit über denselben Schalter deaktivieren. Wenn
deaktiviert, wird Sentry **nicht initialisiert** und es werden keine Netzwerkanfragen gestellt.
Sentrys [Datenschutzrichtlinie](https://sentry.io/privacy/) gilt für empfangene Daten.

---

## Was wir NICHT sammeln

- Kein Benutzerkonto, keine E-Mail-Adresse, kein Passwort
- Keine GPS- oder Standortdaten
- Kein Zugriff auf Kontakte, Kalender, Kamera oder Mikrofon
- Keine Tracker von Dritten (Firebase, Google Analytics, Facebook Pixel usw.)
- Keine Werbe-Identifikatoren (IDFA)
- Kein Videotracking, kein Device-Fingerprinting

---

## Deine Rechte (DSGVO)

Du hast nach der Datenschutz-Grundverordnung folgende Rechte:

**Auskunftsrecht (Art. 15):** Alle deine Daten sind lokal auf deinem Gerät gespeichert.
Du hast volle Einsicht über:
- Einstellungen → Meine Trainingseinheiten (alle bisherigen Runden)
- Einstellungen → Meine Ziele (alle aktiven und archivierten Ziele)
- Einstellungen → Bögen / Pfeilsätze / Orte (Geräteverwaltung)

**Recht auf Datenübertragbarkeit (Art. 20):** Nutze
**Einstellungen → Meine Daten exportieren**, um alle deine Daten als JSON-Datei
herunterzuladen. Die Datei kann über das iOS-Share-Sheet an E-Mail, AirDrop, Dateien
usw. geteilt werden. Dies ist deine komplette Schieß-Historie in einem Standardformat.

**Recht auf Löschung (Art. 17):**
- *Einzelne Trainingseinheit löschen:* Wische die Einheit auf dem Startbildschirm → Löschen
- *Alle Daten löschen:* Deinstalliere JacArrow — iOS löscht automatisch die gesamte
  SQLite-Datenbank und AsyncStorage. Die RevenueCat-Quittung (falls du
  Pro gekauft hast) bleibt bei Apple und RevenueCat für Erstattungs- und Support-Zwecke
  erhalten.

**Recht auf Einschränkung und Widerspruch (Art. 18–21):** JacArrow trifft
keinerlei automatisierte Entscheidungen über dich. Die Smart-Insights-Engine analysiert
nur deine eigenen Trainingsdaten lokal auf deinem Gerät und präsentiert
Beobachtungen — sie trifft keine Entscheidungen in deinem Namen.

**Recht auf Widerruf der Einwilligung (Art. 7):** Das Opt-in für Apple Analytics wird
über die iOS-Einstellungen gesteuert. RevenueCat-Daten werden gelöscht, wenn du deine Apple-ID löschst.

---

## Änderungen

Wir aktualisieren diese Erklärung, wenn wesentliche Änderungen in der Art und Weise auftreten,
wie wir Daten verarbeiten. Änderungen werden kommuniziert über:
1. Datum «Zuletzt aktualisiert» oben auf dieser Seite
2. In-App-Banner beim ersten Start nach dem Update, wenn die Änderung wesentlich ist
   (z. B. neue Dritte, neue Datenerhebung)

---

## Beschwerden

Wenn du der Meinung bist, dass wir deine personenbezogenen Daten unter Verletzung der DSGVO
verarbeiten, hast du das Recht, dich bei deiner nationalen Datenschutzbehörde zu beschweren:

- **Deutschland:** [Bundesbeauftragte für den Datenschutz und die Informationsfreiheit (BfDI)](https://www.bfdi.bund.de/)
- **EU/EWR:** Finde deine Behörde unter
  [edpb.europa.eu](https://www.edpb.europa.eu/about-edpb/about-edpb/members_en)

Wir bitten dich, uns zuerst unter galge.vender.0a@icloud.com zu kontaktieren — wir nehmen
alle Datenschutzanfragen ernst.
