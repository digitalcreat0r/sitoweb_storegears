---
layout: document
title: Privacy Policy - PigeonTweak
permalink: /it/policies/privacy-policy-pigeontweak.html
lang: it
back_url: /it/
back_text: Torna alla Home
---
# Privacy Policy - PigeonTweak

*Ultimo aggiornamento: 14 novembre 2026*

**PigeonTweak** è un'applicazione per i merchant Shopify, sviluppata e gestita da **{{ site.author }}** ("lo sviluppatore"), operante come **{{ site.brand }}**. Consente a un cliente autenticato di correggere l'indirizzo di spedizione di un ordine dalla pagina di stato dell'ordine, finché la finestra di modifica del merchant è ancora aperta e l'ordine può ancora essere modificato. Il paese sull'indirizzo resta lo stesso. Questa informativa spiega quali dati l'app consulta, perché e come vengono trattati.

## 1. Titolare del Trattamento dei Dati
Per i dati di contatto e di supporto descritti in questa informativa, il titolare del trattamento è:

**{{ site.author }} ({{ site.brand }})**

Email: {{ site.email }}<br>
Sito web: {{ site.url }}

Per i dati del negozio e per i dati dei clienti che PigeonTweak legge o aggiorna nel tuo negozio Shopify (compresi nome, indirizzo di spedizione e numero di telefono di un cliente su un ordine), il titolare del trattamento sei tu (il merchant), mentre lo sviluppatore agisce come responsabile del trattamento e tratta tali dati solo per fornire il servizio che hai installato.

## 2. Raccolta delle Informazioni
PigeonTweak tratta informazioni personali sui tuoi clienti solo affinché un cliente titolare di un ordine possa correggere l'indirizzo di spedizione di quell'ordine, e affinché tu possa essere informato che l'indirizzo è cambiato. Non costruisce un elenco di clienti e non legge gli indirizzi email dei clienti da Shopify.

### Dati del negozio e degli ordini consultati tramite Shopify
Quando installi l'app, le concedi i seguenti permessi di accesso (scope):

- **`read_orders`:** Utilizzato per leggere l'ordine che il cliente sta visualizzando: nome e id dell'ordine, se è annullato o chiuso, quando è stato creato, l'indirizzo di spedizione attuale (nome, azienda, via, città, provincia, codice postale, paese e telefono), lo stato di evasione e il totale dell'ordine. È così che l'app decide se una correzione è ancora consentita e quale indirizzo mostrare.
- **`write_orders`:** Utilizzato solo per salvare sull'ordine l'indirizzo di spedizione che il cliente invia. L'app non modifica le righe dell'ordine, gli sconti o i prodotti. Shopify può ricalcolare la spedizione dopo la modifica dell'indirizzo; l'app legge il totale dell'ordine prima e dopo, così da poterti dire se il totale è cambiato.
- **`read_customers`:** Utilizzato affinché il token di sessione del cliente identifichi il cliente autenticato e affinché l'app possa confermare che questo cliente è il titolare dell'ordine. Un ordine ospite senza account cliente non può essere modificato qui. L'app non legge l'indirizzo email del cliente, il numero di telefono dal profilo del cliente né le preferenze di marketing.
- **`read_merchant_managed_fulfillment_orders`:** Utilizzato per leggere se una richiesta di evasione è già stata inviata o accettata. Una volta che lo è, l'indirizzo non può più essere modificato.
- **`write_app_proxy`:** Utilizzato affinché il modulo sulla pagina di stato dell'ordine possa chiamare l'app attraverso il dominio del tuo negozio.

Nome, indirizzo di spedizione e telefono sono dati protetti del cliente. L'app li richiede solo per questo flusso di correzione.

L'app legge inoltre i dati di base del negozio: nome del negozio, dominio del negozio, indirizzo email del negozio e fuso orario. L'email del negozio è l'indirizzo a cui vengono inviate le notifiche al merchant. Viene letta da Shopify quando viene inviata una notifica e non viene copiata nelle impostazioni dell'app. Il fuso orario serve ad applicare le tue ore di silenzio.

### Dati forniti dal cliente
Sulla pagina di stato dell'ordine, il cliente autenticato può inviare un nuovo indirizzo di spedizione. I campi che lasci abilitati possono includere nome, cognome, azienda, indirizzo, città, provincia o stato, codice postale e telefono. Il paese non può essere modificato. L'app verifica che il cliente sia il titolare dell'ordine, che la tua finestra di modifica sia ancora aperta, che nulla sia stato evaso e che nessuna richiesta di evasione sia stata inviata o accettata. Quindi scrive l'indirizzo sull'ordine in Shopify.

### Dati forniti da te nell'app
- **Impostazioni:** Se le correzioni sono abilitate, la finestra di modifica (da 1 ora a 30 giorni), quali campi dell'indirizzo mostra il modulo, se inviarti un'email quando un indirizzo cambia, se inviarti un'email solo quando cambia anche il totale dell'ordine e le ore di silenzio facoltative.

### Dati generati dall'app
- **Registro delle correzioni:** Per ogni tentativo, l'app memorizza il dominio del tuo negozio, l'id dell'ordine Shopify, l'esito (ad esempio, aggiornato o non consentito) e l'orario. Questo registro non memorizza il nome, l'indirizzo o il telefono del cliente. Serve a mostrarti quante correzioni sono andate a buon fine. Le voci più vecchie di 90 giorni vengono eliminate.
- **Notifica al merchant in attesa:** Se attivi le ore di silenzio, una notifica che ricade in quelle ore viene conservata fino al termine del periodo di silenzio. La notifica conservata contiene il nome dell'ordine, l'id dell'ordine Shopify, l'indirizzo di spedizione precedente e quello nuovo (compresi nome e telefono) e il totale dell'ordine prima e dopo la modifica. Viene eliminata dopo l'invio dell'email.
- **Registri tecnici:** Sessioni di autenticazione del tuo negozio (dominio del negozio, token di accesso, scope concessi e, per una sessione online dello staff, id utente Shopify, nome ed email del membro dello staff) e un conteggio delle email di prova inviate oggi, così che l'app possa funzionare e limitare gli invii di prova a tre al giorno.

### Supporto e feedback (volontario)
Se contatti lo sviluppatore via email, puoi fornire volontariamente il tuo nome, il tuo indirizzo email e il dominio del tuo negozio. Queste informazioni vengono utilizzate esclusivamente per rispondere alla tua richiesta e risolvere problemi tecnici. Non vengono utilizzate per nessun altro scopo.

### Analisi, pubblicità e tracciamento
PigeonTweak **non** utilizza strumenti di analisi di terze parti, tracker pubblicitari né profilazione. Non vende né condivide i tuoi dati, né i dati dei tuoi clienti, per finalità di marketing. Il conteggio delle correzioni nell'admin dell'app è calcolato dal registro delle correzioni descritto sopra.

## 3. Come viene salvata una correzione e come vieni avvisato
Il nuovo indirizzo viene scritto sull'ordine nel tuo admin Shopify. Non viene conservato come rubrica separata nell'app.

Se le notifiche al merchant sono attive, l'app invia un'email all'indirizzo email del tuo negozio. Il messaggio indica l'ordine e include l'indirizzo precedente e il nuovo indirizzo. Se il totale dell'ordine è cambiato e hai chiesto di esserne informato, il messaggio include anche il totale precedente e il nuovo totale, e un link all'ordine nell'admin di Shopify. Un'email di prova usa solo dati di esempio e non legge un ordine.

- **Email:** Inviata tramite **Resend** (resend.com). L'indirizzo email del tuo negozio e la notifica (compresi nome del cliente, indirizzo di spedizione e numero di telefono su quell'ordine) vengono trattati da Resend solo per consegnare il messaggio. Consulta l'[Informativa sulla Privacy di Resend](https://resend.com/legal/privacy-policy).
- **Ore di silenzio:** Una notifica che ricade nelle ore che scegli viene trattenuta nel database dell'app e inviata al termine di quella finestra. Gli orari seguono il fuso orario del tuo negozio.

## 4. Servizi di terze parti
- **Shopify:** PigeonTweak viene eseguito all'interno dell'admin di Shopify e sulla pagina di stato dell'ordine, e utilizza la Shopify Admin API e i token di sessione dell'account cliente. Shopify tratta i dati in conformità con la propria [Informativa sulla Privacy](https://www.shopify.com/legal/privacy). L'indirizzo di spedizione è memorizzato sull'ordine in Shopify, secondo i termini di Shopify e le policy del tuo negozio.
- **Resend:** Consegna delle notifiche al merchant, come descritto sopra.
- **Hosting:** L'app è ospitata su Fly.io. Il suo database è un file SQLite su un volume cifrato nella regione primaria dell'app (Chicago, Stati Uniti). L'host conserva i dati per conto dello sviluppatore per eseguire il servizio.

## 5. Archiviazione, sicurezza e conservazione dei dati
I dati dell'app sono archiviati in un database SQLite su un volume cifrato. I dati vengono trasmessi tramite connessioni cifrate (HTTPS) e l'accesso è limitato allo sviluppatore.

- **Uso attivo:** Impostazioni del negozio, sessioni e registro delle correzioni vengono conservati finché l'app è installata, affinché le correzioni e il conteggio delle correzioni continuino a funzionare. Le voci del registro delle correzioni vengono eliminate dopo 90 giorni. Una notifica al merchant in attesa viene conservata solo fino all'invio dell'email, poi eliminata.
- **Disinstallazione:** Quando disinstalli PigeonTweak, l'app riceve la notifica `app/uninstalled` di Shopify ed elimina i dati che detiene per il tuo negozio: sessioni, impostazioni del negozio, registro delle correzioni e qualsiasi notifica al merchant ancora in attesa per le ore di silenzio.
- **Richieste di conformità Shopify:** L'app gestisce i webhook obbligatori sulla privacy di Shopify. `shop/redact` viene inviato circa 48 ore dopo la disinstallazione ed elimina gli eventuali dati del negozio ancora conservati. `customers/redact` elimina il registro delle correzioni e qualsiasi notifica in attesa per gli ordini indicati nella richiesta. L'app non conserva un profilo del cliente. Con `customers/data_request`, se una voce del registro delle correzioni o una notifica in attesa corrisponde agli ordini della richiesta, quei dati vengono inviati via email all'indirizzo email del negozio. Se non è conservato nulla, non ci sono dati dei clienti da restituire.
- **Cosa non viene copiato fuori da Shopify:** L'app non conserva una copia duratura dell'indirizzo di spedizione. Dopo l'invio di una notifica, o dopo la disinstallazione, l'indirizzo resta sull'ordine in Shopify, che controlli tu. Il registro delle correzioni conserva l'id dell'ordine e l'orario, non l'indirizzo.
- **Email di supporto:** Conservate solo per il tempo necessario a gestire la tua richiesta e poi eliminate, salvo che la legge richieda un periodo più lungo.

## 6. Incidenti di sicurezza
Lo sviluppatore è responsabile del contenimento di un incidente di sicurezza che esponga nome del cliente, indirizzo di spedizione, numero di telefono o dati dell'ordine trattati dall'app. Se lo sviluppatore viene a conoscenza di un tale incidente, lo contiene e avvisa Shopify all'indirizzo [security@shopify.com](mailto:security@shopify.com) entro 24 ore. I merchant interessati vengono avvisati come richiesto dalla legge applicabile.

## 7. Trasferimenti internazionali di dati
Lo sviluppatore e i fornitori di servizi sopra elencati possono trattare i dati in paesi diversi dal tuo, anche negli Stati Uniti e al di fuori dello Spazio Economico Europeo. In tal caso vengono applicate garanzie adeguate (come le Clausole Contrattuali Standard) come richiesto dalla legge applicabile.

## 8. Conformità e diritti
In conformità con il GDPR, il UK GDPR, il CCPA/CPRA e le altre leggi applicabili sulla privacy, gli interessati hanno il diritto di accedere, rettificare, cancellare, limitare o esportare i propri dati e di opporsi al loro trattamento. Tali diritti si esercitano come segue:

- **Dati del tuo negozio:** Modifica o cancella le impostazioni nell'app in qualsiasi momento, oppure disinstalla l'app per eliminare le sessioni, le impostazioni, il registro delle correzioni e qualsiasi notifica in attesa descritti nella Sezione 5. Contatta lo sviluppatore per altre richieste.
- **Dati dei tuoi clienti:** Sei il titolare del trattamento dei dati degli ordini dei clienti. Un cliente deve contattare il tuo negozio in merito a un ordine. Se una richiesta riguarda qualcosa che l'app detiene ancora (una notifica in attesa, o un id ordine nel registro delle correzioni), Shopify invia `customers/data_request` o `customers/redact`, e puoi anche contattare lo sviluppatore all'indirizzo email indicato di seguito indicando il dominio del negozio. Le richieste ricevono risposta entro 30 giorni.

PigeonTweak non vende né condivide informazioni personali e non adotta decisioni automatizzate che producano effetti giuridici o analogamente significativi. Hai inoltre il diritto di presentare un reclamo all'autorità locale per la protezione dei dati.

## 9. Privacy dei minori
PigeonTweak è uno strumento professionale per i merchant Shopify e non è rivolto ai minori. Lo sviluppatore non raccoglie consapevolmente informazioni personali da persone di età inferiore ai 16 anni, al di là dei dati di spedizione che un cliente invia su un ordine che il merchant già detiene.

## 10. Modifiche a questa informativa
Questa informativa può essere aggiornata di tanto in tanto, ad esempio quando cambiano le funzionalità dell'app. La data di "Ultimo aggiornamento" in alto indica la revisione più recente. Le modifiche significative saranno comunicate tramite l'app o via email.

## 11. Informazioni di contatto
Per qualsiasi domanda riguardante la tua privacy, puoi contattare lo sviluppatore all'indirizzo:<br>
**{{ site.email }}**
