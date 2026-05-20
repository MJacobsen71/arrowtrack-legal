# Support — ArrowTrack

**Zuletzt aktualisiert:** 2026-05-20
**Abgedeckte Version:** v1.0+
**Kontakt:** galge.vender.0a@icloud.com

---

## Schnelle Hilfe

### Wie nehme ich eine Passe auf?

1. Öffne ArrowTrack → tippe **Neue Trainingseinheit** im Home-Tab
2. Wähle Ort, Auflage und Rundenformat → tippe **Trainingseinheit starten**
3. **Tippe auf die Auflage**, um jeden Pfeil zu platzieren — nutze Pinch-Zoom und die Präzisionslupe für Genauigkeit
4. Tippe **Passe speichern**, wenn alle Pfeile platziert sind
5. Wiederhole für jede Passe, bis die Runde abgeschlossen ist

### Was ist der Unterschied zwischen X und 10?

Der X-Ring ist der innerste Ring und zählt 10 Punkte — genau wie der 10er-Ring. ArrowTrack trackt das X separat, da das X im Wettkampf als Tiebreaker verwendet wird. Tippe die «X»-Taste, wenn ein Pfeil im Score-Pad-Modus den X-Ring trifft.

### Wie korrigiere ich einen falsch platzierten Pfeil?

1. Drücke lange auf den Pfeil auf der Auflage → die Präzisionslupe aktiviert sich
2. Ziehe den Pfeil an die neue Position → loslassen
3. ODER tippe auf den Pfeil zum Auswählen → tippe **Löschen**, um ihn zu entfernen

Im Score-Pad-Modus: Tippe das Pfeil-Badge im Score-Pad und wähle einen neuen Wert.

### Was ist die Nachregistrierung (das 📋-Symbol)?

Das 📋-Symbol markiert Trainingseinheiten, die manuell mit dem Score-Pad eingegeben wurden, statt mit Koordinaten auf der Auflage erfasst zu werden. Trefferbild, Konstellation und Streuungsanalyse sind für nachregistrierte Einheiten nicht verfügbar — nur die Punktsummen.

### Wie kaufe ich Pro?

1. Tippe eine Pro-geschützte Funktion an (z. B. ein Theme mit Pro-Badge)
2. Das Paywall erscheint mit der Schaltfläche **Pro kaufen (299 NOK)**
3. Apples Standard-Kaufdialog erscheint → bestätige mit Face ID / Passcode
4. Pro wird sofort aktiviert — alle Funktionen werden freigeschaltet

**Preis:** 299 NOK Einmalkauf, lebenslang. Kein Abonnement, keine wiederkehrenden Belastungen.

### Wie stelle ich Käufe auf einem neuen iPhone wieder her?

1. Lade ArrowTrack auf dem neuen iPhone herunter (kostenlose Version)
2. Melde dich mit derselben Apple-ID an, mit der du Pro gekauft hast
3. Öffne ArrowTrack → **Einstellungen → Lizenz → Käufe wiederherstellen**
4. Pro wird automatisch reaktiviert

Wenn du die Apple-ID gewechselt hast: kontaktiere galge.vender.0a@icloud.com, und wir helfen dir.

### Wie exportiere ich meine Daten?

**Einstellungen → Über die App → Meine Daten exportieren** → das iOS-Share-Sheet erscheint. Wähle AirDrop, Mail, Dateien oder wohin auch immer du die JSON-Datei senden möchtest.

Die JSON enthält alle Trainingseinheiten, Runden, Pfeile, Ziele, Bogen-Setups und Einstellungen — vollständige Portabilität nach DSGVO Art. 20.

### Wie lösche ich alle meine Daten?

Deinstalliere ArrowTrack → iOS entfernt automatisch die gesamte SQLite-Datenbank und alle Einstellungen. Auf dem Gerät verbleiben keine Restdaten.

Wenn du Pro gekauft hast: die Quittung bleibt bei Apple (für Erstattungs- und Support-Zwecke). Die Deinstallation hat keinen Einfluss auf zukünftige Neuinstallationen — Pro reaktiviert sich automatisch über Käufe wiederherstellen.

### Welche Rundenformate werden unterstützt?

- **WA 720** (Outdoor, 6 Passen × 12 Pfeile = 72 Pfeile)
- **WA 18 m Halle** (10 Passen × 3 Pfeile)
- **WA 1440** (4 sequentielle Distanzen)
- **Vegas Shoot** (10 Passen × 3 Pfeile Halle 18 m)
- **AGB Portsmouth** (10 Passen × 3 Pfeile Halle 20 yd)
- **NFAA Indoor** (12 Passen × 5 Pfeile Halle 20 yd)
- **Freies Training** (keine Format-Grenzen)

Alle Formate folgen offizieller WA-Book-3-Compliance: Linienberührungsregel, separates X-Tracking, korrekte Ring-Radien.

### Welche Auflagen werden unterstützt?

- **WA 122 cm 10-Ring** (Outdoor-Standard)
- **WA 80 cm 10-Ring** (Outdoor Langdistanz)
- **WA 40 cm 10-Ring** (Halle Single-Spot)
- **WA 40 cm Vegas 3-Spot triangulär** (Hallenwettkampf)
- **WA 40 cm Vegas 3-Spot vertikal** (Halle Alternative)
- **AGB Portsmouth 60 cm 10-Ring** (Halle UK)
- **NFAA Halle Single-Spot blau 40 cm** (USA)
- **NFAA Halle 5-Spot blau 40 cm** (USA Wettkampf)

---

## Technische Probleme

### Die App stürzt beim Start ab

1. Schalte das iPhone aus und wieder ein
2. Wenn weiterhin Probleme: deinstalliere und installiere ArrowTrack neu (Kaufdaten gehen NICHT verloren — die Quittung bleibt bei Apple)
3. Sende das Crash-Log an galge.vender.0a@icloud.com: **Einstellungen → Datenschutz & Sicherheit → Analyse & Verbesserungen → Analysedaten** → finde das ArrowTrack-Log → teile es mit uns

Wenn du dich entschieden hast, Analytics über iOS mit dem Entwickler zu teilen, werden Crash-Logs automatisch an uns gesendet.

### Punktdaten sind nach einem Update verschwunden

ArrowTrack speichert alles lokal in SQLite. Updates migrieren die Datenbank vorwärtsgerichtet — alte Daten werden ins neue Format konvertiert, niemals gelöscht.

Falls du Datenverlust erlebst:
1. Verifiziere, dass du mit derselben Apple-ID angemeldet bist
2. Prüfe **Einstellungen → Über die App → Versionsnummer** — ist sie aktuell?
3. Sende uns eine Beschreibung an galge.vender.0a@icloud.com

Wir haben eine strikte Regel, dass veröffentlichte Migrationen unveränderlich sind — Datenverlust durch Updates sollte niemals passieren. Wenn es doch geschieht, haben wir einen Bug und möchten davon erfahren.

### Pinch-Zoom funktioniert nicht auf der Auflage

1. Versuche es mit zwei Fingern, nicht einem
2. Prüfe, dass «Bewegung reduzieren» nicht aktiviert ist unter **iOS-Einstellungen → Bedienungshilfen → Bewegung** — dies kann Gesten in einigen Apps einschränken
3. App komplett schließen (von unten nach oben wischen, ArrowTrack nach oben wischen) und erneut öffnen

### Die Konstellationsansicht vibriert beim Ziehen

Das war ein Bug in v0.28.2 und früher — behoben in v0.28.3. Aktualisiere die App auf die neueste Version im App Store.

---

## Feedback und Anfragen

### Eine neue Funktion vorschlagen

Sende eine E-Mail an galge.vender.0a@icloud.com mit:
- **Was** du möchtest (kurze Beschreibung)
- **Warum** (was würde es in deinem Training verbessern?)
- **Wie oft** würdest du es nutzen (täglich / pro Trainingseinheit / seltener)

Wir lesen jede einzelne Anfrage und veröffentlichen priorisierte Funktionen im «Was ist neu»-Stream der App.

### Einen Bug melden

Sende eine E-Mail an galge.vender.0a@icloud.com mit:
- **Was schiefgelaufen ist** (so detailliert wie möglich)
- **Was du erwartet hast**
- **Schritt-für-Schritt** zur Reproduktion
- **iOS-Version** und **iPhone-Modell** (Einstellungen → Allgemein → Info)
- **ArrowTrack-Version** (Einstellungen → Über die App)
- Screenshot, falls relevant

### Allgemein
Wir antworten auf alle Anfragen innerhalb von 3 Werktagen. Dringende Probleme (Abstürze, die dich am Schießen hindern) werden höher priorisiert.

---

## DSGVO und Datenschutz

Für die vollständige Datenschutzerklärung: [Datenschutz](https://mjacobsen71.github.io/arrowtrack-legal/privacy-de)

Um deine Daten zu exportieren, eine Trainingseinheit zu löschen oder andere DSGVO-Rechte auszuüben: siehe die Datenschutzerklärung.

Datenschutzbeschwerden: kontaktiere uns **zuerst** unter galge.vender.0a@icloud.com. Falls wir die Angelegenheit nicht lösen können, kannst du dich an deine nationale Datenschutzbehörde wenden. Für Deutschland: [BfDI](https://www.bfdi.bund.de/).

---

## Über ArrowTrack

**Entwickler:** Morten Jacobsen, Norwegen
**Homepage:** [mjacobsen71.github.io/arrowtrack-legal](https://mjacobsen71.github.io/arrowtrack-legal)
**Datenschutzerklärung:** [Datenschutz](https://mjacobsen71.github.io/arrowtrack-legal/privacy-de)
**Lizenzen (Open Source):** siehe Einstellungen → Über die App → Lizenzen in der App

ArrowTrack ist ein Solo-Entwickler-Projekt, gebaut für Bogenschützen auf jedem Niveau — vom ersten Pfeil bis zum hundertsten Turnier. WA Book 3-konformes Scoring ist von Tag eins an dabei, bereit, wenn du es brauchst. Erstellt mit React Native + Expo + TypeScript + SQLite. Kein Backend, keine Cloud, kein Tracking.

Danke, dass du die App nutzt. 🏹
