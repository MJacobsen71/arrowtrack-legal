# Supporto — ArrowTrack

**Ultimo aggiornamento:** 2026-05-20
**Versione coperta:** v1.0+
**Contatto:** galge.vender.0a@icloud.com

---

## Aiuto rapido

### Come registro una volée?

1. Apri ArrowTrack → tocca **Nuova sessione** nella scheda Home
2. Scegli luogo, visuale e formato del round → tocca **Avvia sessione**
3. **Tocca sulla visuale** per posizionare ogni freccia — usa il pinch-zoom e la lente di precisione per maggiore accuratezza
4. Tocca **Salva volée** quando tutte le frecce sono posizionate
5. Ripeti per ogni volée finché il round non è completo

### Qual è la differenza tra X e 10?

L'X-ring è il cerchio più interno e vale 10 punti — uguale al 10. ArrowTrack traccia l'X separatamente perché viene usato come spareggio nelle competizioni. Tocca il pulsante «X» quando una freccia colpisce l'X-ring in modalità score-pad.

### Come correggo una freccia mal posizionata?

1. Premi a lungo sulla freccia sulla visuale → si attiva la lente di precisione
2. Trascina la freccia nella nuova posizione → rilascia
3. OPPURE tocca la freccia per selezionarla → tocca **Elimina** per rimuoverla

In modalità score-pad: tocca il badge della freccia nello score-pad e scegli un nuovo valore.

### Cos'è la post-registrazione (l'icona 📋)?

L'icona 📋 indica sessioni inserite manualmente con lo score-pad, non registrate sulla visuale con le coordinate. Mappa degli impatti, costellazione e analisi della dispersione non sono disponibili per le sessioni post-registrate — solo i totali del punteggio.

### Come acquisto Pro?

1. Tocca una funzione bloccata con Pro (es. un tema con il badge Pro)
2. Appare il paywall con il pulsante **Acquista Pro (299 NOK)**
3. Compare il modale di acquisto standard di Apple → conferma con Face ID / passcode
4. Pro si attiva immediatamente — tutte le funzioni si sbloccano

**Prezzo:** 299 NOK acquisto una tantum, a vita. Nessun abbonamento, nessun addebito ricorrente.

### Come ripristino gli acquisti su un nuovo iPhone?

1. Scarica ArrowTrack sul nuovo iPhone (versione gratuita)
2. Accedi con lo stesso ID Apple usato per acquistare Pro
3. Apri ArrowTrack → **Impostazioni → Licenza → Ripristina acquisti**
4. Pro si riattiva automaticamente

Se hai cambiato ID Apple: contatta galge.vender.0a@icloud.com e ti aiuteremo.

### Come esporto i miei dati?

**Impostazioni → Sull'app → Esporta i miei dati** → appare il foglio di condivisione iOS. Scegli AirDrop, Mail, File o dove vuoi inviare il file JSON.

Il JSON contiene tutte le sessioni, i round, le frecce, gli obiettivi, le configurazioni dell'arco e le impostazioni — portabilità completa ai sensi dell'art. 20 GDPR.

### Come elimino tutti i miei dati?

Disinstalla ArrowTrack → iOS rimuove automaticamente l'intero database SQLite e tutte le impostazioni. Nessun dato residuo rimane sul dispositivo.

Se hai acquistato Pro: la ricevuta rimane presso Apple (per scopi di rimborso e supporto). La disinstallazione non influisce sulle reinstallazioni future — Pro si riattiva automaticamente tramite Ripristina acquisti.

### Quali formati di round sono supportati?

- **WA 720** (outdoor, 6 volée × 12 frecce = 72 frecce)
- **WA 18 m indoor** (10 volée × 3 frecce)
- **WA 1440** (4 distanze sequenziali)
- **Vegas Shoot** (10 volée × 3 frecce indoor 18 m)
- **AGB Portsmouth** (10 volée × 3 frecce indoor 20 yd)
- **NFAA Indoor** (12 volée × 5 frecce indoor 20 yd)
- **Allenamento libero** (nessun limite di formato)

Tutti i formati seguono la conformità ufficiale WA Book 3: regola della linea, tracciamento separato dell'X, raggi degli anelli corretti.

### Quali visuali sono supportate?

- **Visuale WA 122 cm 10-ring** (standard outdoor)
- **Visuale WA 80 cm 10-ring** (outdoor lunga distanza)
- **Visuale WA 40 cm 10-ring** (indoor, singolo spot)
- **Visuale WA 40 cm Vegas 3-spot triangolare** (gara indoor)
- **Visuale WA 40 cm Vegas 3-spot verticale** (alternativa indoor)
- **Visuale AGB Portsmouth 60 cm 10-ring** (indoor UK)
- **Visuale NFAA indoor singolo spot blu 40 cm** (USA)
- **Visuale NFAA indoor 5-spot blu 40 cm** (gara USA)

---

## Problemi tecnici

### L'app si blocca all'avvio

1. Spegni e riaccendi l'iPhone
2. Se persiste: disinstalla e reinstalla ArrowTrack (i dati di acquisto NON vengono persi — la ricevuta rimane presso Apple)
3. Invia il log del crash a galge.vender.0a@icloud.com: **Impostazioni → Privacy e sicurezza → Analisi e miglioramenti → Dati di analisi** → trova il log di ArrowTrack → condividilo con noi

Se hai scelto di condividere l'analisi con lo sviluppatore tramite iOS, i log dei crash ci vengono inviati automaticamente.

### I dati di punteggio sono spariti dopo un aggiornamento

ArrowTrack memorizza tutto localmente in SQLite. Gli aggiornamenti migrano il database solo in avanti — i vecchi dati vengono convertiti nel nuovo formato, mai eliminati.

Se riscontri perdita di dati:
1. Verifica di essere connesso con lo stesso ID Apple
2. Controlla **Impostazioni → Sull'app → Numero di versione** — è aggiornato?
3. Inviaci una descrizione a galge.vender.0a@icloud.com

Abbiamo una regola ferrea che le migrazioni pubblicate sono immutabili — la perdita di dati dagli aggiornamenti non dovrebbe mai accadere. Se accade, abbiamo un bug e vogliamo saperlo.

### Il pinch-zoom non funziona sulla visuale

1. Prova con due dita, non una
2. Verifica che «Riduci movimento» non sia attivato in **Impostazioni iOS → Accessibilità → Movimento** — può limitare le gesture in alcune app
3. Chiudi l'app completamente (scorri verso l'alto dal basso, scorri ArrowTrack verso l'alto) e riapri

### La costellazione vibra durante il trascinamento

Era un bug in v0.28.2 e precedenti — risolto in v0.28.3. Aggiorna l'app alla versione più recente sull'App Store.

---

## Feedback e richieste

### Suggerisci una nuova funzione

Invia un'email a galge.vender.0a@icloud.com con:
- **Cosa** vuoi (breve descrizione)
- **Perché** (cosa migliorerebbe nel tuo allenamento?)
- **Quanto spesso** la useresti (giornalmente / a sessione / meno frequentemente)

Leggiamo ogni singola richiesta e pubblichiamo le funzioni prioritizzate nello stream «Novità» dell'app.

### Segnala un bug

Invia un'email a galge.vender.0a@icloud.com con:
- **Cosa è andato storto** (più dettagliato possibile)
- **Cosa ti aspettavi che succedesse**
- **Passo per passo** per riprodurlo
- **Versione iOS** e **modello di iPhone** (Impostazioni → Generali → Info)
- **Versione di ArrowTrack** (Impostazioni → Sull'app)
- Screenshot se rilevante

### Generale
Rispondiamo a tutte le richieste entro 3 giorni lavorativi. I problemi urgenti (crash che ti impediscono di tirare) hanno priorità più alta.

---

## GDPR e privacy

Per l'informativa sulla privacy completa: [Privacy](https://mjacobsen71.github.io/arrowtrack-legal/privacy-it)

Per esportare i tuoi dati, eliminare una sessione o esercitare altri diritti GDPR: vedi l'Informativa sulla privacy.

Reclami sulla privacy: contattaci **prima** a galge.vender.0a@icloud.com. Se non riusciamo a risolvere la questione, puoi presentare reclamo alla tua autorità nazionale di protezione dei dati. Per l'Italia: [Garante per la protezione dei dati personali](https://www.garanteprivacy.it/).

---

## Su ArrowTrack

**Sviluppatore:** Morten Jacobsen, Norvegia
**Sito web:** [mjacobsen71.github.io/arrowtrack-legal](https://mjacobsen71.github.io/arrowtrack-legal)
**Informativa sulla privacy:** [Privacy](https://mjacobsen71.github.io/arrowtrack-legal/privacy-it)
**Licenze (open source):** vedi Impostazioni → Sull'app → Licenze nell'app

ArrowTrack è un progetto di un singolo sviluppatore, costruito per arcieri che prendono sul serio le regole di World Archery. Costruito con React Native + Expo + TypeScript + SQLite. Niente backend, niente cloud, niente tracciamento.

Grazie per aver usato l'app. 🏹
