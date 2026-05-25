# Informativa sulla privacy — JacArrow

**Ultimo aggiornamento:** 2026-05-25
**Titolare del trattamento:** Morten Jacobsen, Norvegia
**Contatto:** galge.vender.0a@icloud.com

---

## Versione breve

JacArrow memorizza **tutti i tuoi dati localmente sul tuo dispositivo**. Non abbiamo alcun
server che riceva i tuoi tiri, le tue sessioni o i tuoi obiettivi. Quando disinstalli
l'app, tutti i dati spariscono.

Le uniche terze parti che ricevono informazioni sono:
- **Apple** — gestisce gli acquisti su App Store e le notifiche
- **RevenueCat** (dopo l'acquisto di Pro) — verifica il tuo acquisto
- **Sentry** (solo se attivi le segnalazioni di crash) — riceve dati anonimi sui crash per aiutarci a correggere i bug

Hai i pieni diritti GDPR di accesso, cancellazione e portabilità dei dati.

---

## Cosa memorizziamo

### Sul tuo dispositivo (in locale, non lascia mai il telefono)
- **Dati di tiro:** sessioni, round, posizionamenti delle frecce, punteggi, etichette, obiettivi, archi e set di frecce
- **Impostazioni:** lingua selezionata, tema, mano di tiro, classe di gara, opzioni di notifica
- **Cronologia dell'app:** stato dei coach-mark (suggerimenti già visualizzati), flag di tutorial completati

Tutti questi dati sono memorizzati in un database SQLite e in AsyncStorage sul tuo iPhone.
Né JacArrow né alcuna terza parte ha accesso a questi dati.

### iCloud (solo se iCloud Drive è abilitato)
JacArrow pianifica di utilizzare iCloud Key-Value Storage per uno scopo specifico:
ricordare se hai già iniziato il periodo di prova. Questo si sincronizza
tramite il tuo account iCloud per impedire che disinstallazione + reinstallazione
concedano un nuovo periodo di prova gratuito.

- Apple è il responsabile del trattamento (il nostro accordo è regolato dai loro termini standard)
- I valori memorizzati sono **solo**: la data di inizio della prova e uno stato «prova utilizzata»
- Questa funzione si attiverà quando lanceremo il modello Pro (Fase 4b)

Se hai disabilitato iCloud Drive, o disabilitato iCloud Drive specificamente
per JacArrow, iCloud non viene utilizzato.

---

## Terze parti

### Apple App Store
Tutti gli acquisti in-app sono gestiti da Apple. Non riceviamo mai informazioni sulla
carta, indirizzi o altri dettagli di pagamento. La
[politica sulla privacy di Apple](https://www.apple.com/it/legal/privacy/) si applica al
processo di acquisto.

### Apple Push Notification Service (APNS)
JacArrow invia notifiche locali (RP raggiunto, scadenza del periodo di prova,
promemoria degli obiettivi). Per recapitarle, iOS registra un token di dispositivo anonimo
con Apple. Non abbiamo alcun server che invii messaggi push — tutte le notifiche
sono generate localmente sul tuo dispositivo in base allo stato dell'app.

### RevenueCat (solo dopo l'acquisto di Pro)
Quando acquisti JacArrow Pro, RevenueCat registra la tua ricevuta e un
`appUserId` anonimo (UUID generato sul tuo dispositivo). Ciò è necessario
affinché l'app possa verificare il tuo acquisto in utilizzi successivi e durante il
«Ripristina acquisti». La
[politica sulla privacy di RevenueCat](https://www.revenuecat.com/privacy) si applica. Non inviamo mai
il tuo nome, la tua email o altri dati personali.

### Apple Analytics / Segnalazioni di crash
Se hai abilitato «Condividi analisi app» nelle Impostazioni iOS, Apple invia
dati aggregati anonimi su utilizzo e crash allo sviluppatore.
JacArrow utilizza questi dati per la correzione dei bug e l'ottimizzazione delle prestazioni. Puoi
disabilitarlo tramite:
**Impostazioni iOS → Privacy e sicurezza → Analisi e miglioramenti**.

### Sentry (solo se hai abilitato le segnalazioni di crash)
Sentry è un servizio di monitoraggio degli errori che ci aiuta a identificare e
correggere i bug in JacArrow. Sentry riceve dati solo se hai dato
**esplicito consenso** tramite **Impostazioni → Privacy → Segnalazioni di crash**
(l'interruttore è disattivato per impostazione predefinita).

Quando attivato, vengono inviati ai server europei di Sentry (Germania):
- Stack trace dei crash (nomi file, numeri di riga, tipi di eccezione)
- Modello del dispositivo e versione iOS
- Versione dell'app e numero di build

**Non** inviamo:
- Informazioni personali (nessun nome, nessuna email, nessun ID utente collegato all'identità)
- Trace di performance o transazioni (`tracesSampleRate: 0`)
- Indirizzi IP (`sendDefaultPii: false`)

Puoi disattivare le segnalazioni di crash in qualsiasi momento tramite lo stesso interruttore. Quando
disattivato, Sentry **non viene inizializzato** e non vengono effettuate richieste di rete.
L'[informativa sulla privacy di Sentry](https://sentry.io/privacy/) si applica ai dati ricevuti.

---

## Cosa NON raccogliamo

- Nessun account utente, indirizzo email o password
- Nessun dato GPS o di posizione
- Nessun accesso a contatti, calendario, fotocamera o microfono
- Nessun tracker di terze parti (Firebase, Google Analytics, Facebook Pixel, ecc.)
- Nessun identificatore pubblicitario (IDFA)
- Nessun video-tracking né fingerprinting del dispositivo

---

## I tuoi diritti (GDPR)

Hai i seguenti diritti ai sensi del Regolamento generale sulla protezione dei dati:

**Diritto di accesso (Art. 15):** Tutti i tuoi dati sono memorizzati localmente sul tuo dispositivo.
Hai piena visibilità tramite:
- Impostazioni → Le mie sessioni (tutti i round storici)
- Impostazioni → I miei obiettivi (tutti gli obiettivi attivi e archiviati)
- Impostazioni → Archi / Set di frecce / Luoghi (gestione attrezzatura)

**Diritto alla portabilità dei dati (Art. 20):** Usa
**Impostazioni → Esporta i miei dati** per scaricare tutti i tuoi dati come file JSON. Il
file può essere condiviso tramite il foglio di condivisione iOS a email, AirDrop, File, ecc.
Questa è la tua cronologia di tiro completa in un formato standard.

**Diritto alla cancellazione (Art. 17):**
- *Eliminare una singola sessione:* fai scorrere la sessione sulla schermata Home → Elimina
- *Eliminare tutti i dati:* disinstalla JacArrow — iOS elimina automaticamente l'intero
  database SQLite e AsyncStorage. La ricevuta RevenueCat (se hai
  acquistato Pro) viene conservata da Apple e RevenueCat per scopi di rimborso e supporto.

**Diritto di limitazione e opposizione (Art. 18–21):** JacArrow non prende
alcuna decisione automatizzata su di te. Il motore Smart Insights analizza solo
i tuoi dati di allenamento localmente sul tuo dispositivo e presenta
osservazioni — non prende decisioni per tuo conto.

**Diritto di revocare il consenso (Art. 7):** L'opt-in di Apple Analytics è controllato
tramite le Impostazioni iOS. I dati RevenueCat vengono eliminati quando elimini il tuo ID Apple.

---

## Modifiche

Aggiorneremo questa informativa in caso di modifiche significative nelle modalità di
trattamento dei dati. Le modifiche sono comunicate tramite:
1. Data «Ultimo aggiornamento» in cima a questa pagina
2. Banner in-app al primo avvio dopo l'aggiornamento se la modifica è sostanziale
   (es. nuove terze parti, nuova raccolta di dati)

---

## Reclami

Se ritieni che stiamo trattando i tuoi dati personali in violazione del GDPR,
hai il diritto di presentare un reclamo alla tua autorità nazionale di protezione dei dati:

- **Italia:** [Garante per la protezione dei dati personali](https://www.garanteprivacy.it/)
- **UE/SEE:** trova la tua autorità su
  [edpb.europa.eu](https://www.edpb.europa.eu/about-edpb/about-edpb/members_en)

Ti invitiamo a contattarci prima a galge.vender.0a@icloud.com — prendiamo
tutte le richieste sulla privacy seriamente.
