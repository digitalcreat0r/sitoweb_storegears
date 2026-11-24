---
layout: document
title: Privacy Policy - PigeonTweak
permalink: /it/policies/privacy-policy-pigeontweak.html
lang: it
back_url: /it/
back_text: Torna alla Home
---
# Privacy Policy - PigeonTweak

*Ultimo aggiornamento: 24 novembre 2026*

**PigeonTweak** è un'applicazione per i merchant Shopify, sviluppata e gestita da **{{ site.author }}** ("lo sviluppatore"), operante come **{{ site.brand }}**. Consente a un cliente autenticato di correggere l'indirizzo di spedizione di un ordine dalla pagina di stato dell'ordine o dalla pagina di ringraziamento, finché la finestra di modifica del merchant è ancora aperta e l'ordine può ancora essere modificato. Il paese sull'indirizzo resta lo stesso. Questa informativa spiega quali dati l'app consulta, perché e come vengono trattati.

## 1. Titolare del Trattamento dei Dati
Per i dati di contatto e di supporto descritti in questa informativa, il titolare del trattamento è:

**{{ site.author }} ({{ site.brand }})**

Email: {{ site.email }}<br>
Sito web: {{ site.url }}

Per i dati del negozio e per i dati dei clienti che PigeonTweak legge o aggiorna nel tuo negozio Shopify (compresi nome, indirizzo di spedizione e numero di telefono di un cliente su un ordine), il titolare del trattamento sei tu (il merchant). Lo sviluppatore agisce come responsabile del trattamento e tratta tali dati solo per fornire il servizio che hai installato.

## 2. Raccolta delle Informazioni
PigeonTweak tratta informazioni personali sui tuoi clienti solo affinché un cliente titolare di un ordine possa correggere l'indirizzo di spedizione di quell'ordine, e affinché tu possa essere informato che l'indirizzo è cambiato. Non costruisce un elenco di clienti e non legge gli indirizzi email dei clienti da Shopify.

### Dati del negozio e degli ordini consultati tramite Shopify
Quando installi l'app, le concedi i seguenti permessi di accesso (scope):

- **`read_orders`:** Utilizzato per leggere l'ordine che il cliente sta visualizzando: nome e id dell'ordine, stato, data di creazione, stato di evasione, totale dell'ordine e indirizzo di spedizione attuale (nome, azienda, via, città, provincia, codice postale, paese e telefono).
- **`write_orders`:** Utilizzato solo per salvare sull'ordine l'indirizzo di spedizione che il cliente invia. L'app non modifica le righe dell'ordine, gli sconti o i prodotti.
- **`read_customers`:** Utilizzato per identificare il cliente autenticato e confermare che sia il titolare dell'ordine. L'app non legge l'indirizzo email del cliente, le preferenze di marketing né altri dati del profilo.
- **`read_merchant_managed_fulfillment_orders` e `read_third_party_fulfillment_orders`:** Utilizzati per leggere se una richiesta di evasione è già stata inviata. Una volta che lo è, l'indirizzo non può più essere modificato.
- **`write_app_proxy`:** Utilizzato affinché il modulo dell'ordine possa chiamare l'app attraverso il dominio del tuo negozio.

Nome, indirizzo di spedizione e telefono sono dati protetti del cliente. L'app li richiede solo per questo flusso di correzione.

L'app legge inoltre il nome del negozio, il dominio del negozio, l'indirizzo email del negozio e il fuso orario. L'email del negozio è l'indirizzo a cui vengono inviate le notifiche al merchant, mentre il fuso orario serve ad applicare le tue ore di silenzio.

### Dati forniti dal cliente
Il cliente autenticato può inviare un nuovo indirizzo di spedizione (nome, cognome, azienda, indirizzo, città, provincia o stato, codice postale e telefono, in base ai campi che abiliti). L'app verifica l'ordine e le tue impostazioni, quindi scrive l'indirizzo sull'ordine in Shopify.

### Dati forniti da te nell'app
Le tue impostazioni: se le correzioni sono abilitate, la finestra di modifica, quali campi dell'indirizzo mostra il modulo e le preferenze su notifiche email e ore di silenzio.

### Dati generati dall'app
- **Conteggio delle correzioni:** Un conteggio giornaliero delle correzioni riuscite per il tuo negozio (dominio del negozio, data, numero). Non contiene id dell'ordine, nome, indirizzo o telefono. Viene eliminato dopo circa 30 giorni.
- **Dati trattenuti temporaneamente:** Se una correzione cambia il totale dell'ordine, l'app conserva per alcuni minuti l'indirizzo precedente e la notifica (compresi nome e telefono), così che il cliente possa annullare la modifica. Le notifiche ritardate dalle tue ore di silenzio vengono conservate fino all'invio. Questi dati vengono eliminati una volta gestiti, e comunque entro 90 giorni.
- **Registro degli accessi:** L'app registra quando il nome, l'indirizzo o il telefono di un cliente vengono letti, salvati, esportati o eliminati (dominio del negozio, id dell'ordine, azione e id del cliente). Non memorizza nome, indirizzo o telefono. Viene eliminato dopo 90 giorni.
- **Registri tecnici:** Sessioni di autenticazione del tuo negozio (dominio del negozio, token di accesso, scope concessi e, per una sessione online dello staff, id utente Shopify, nome ed email del membro dello staff) e un conteggio giornaliero delle email di prova.

### Supporto e feedback (volontario)
Se contatti lo sviluppatore via email, puoi fornire il tuo nome, il tuo indirizzo email e il dominio del tuo negozio. Queste informazioni vengono utilizzate esclusivamente per rispondere alla tua richiesta e risolvere problemi tecnici.

### Analisi, pubblicità e tracciamento
PigeonTweak **non** utilizza strumenti di analisi di terze parti, tracker pubblicitari né profilazione. Non vende né condivide i tuoi dati, né i dati dei tuoi clienti, per finalità di marketing.

## 3. Notifiche al merchant
Se le notifiche al merchant sono attive, l'app invia un'email all'indirizzo email del tuo negozio quando un indirizzo cambia. Il messaggio include il nome dell'ordine, l'indirizzo precedente e quello nuovo (compresi nome e telefono) e, se il totale dell'ordine è cambiato, il totale precedente e il nuovo totale. L'email viene inviata tramite **Resend** (resend.com), che tratta questi dati solo per consegnare il messaggio. Consulta l'[Informativa sulla Privacy di Resend](https://resend.com/legal/privacy-policy).

## 4. Servizi di terze parti
- **Shopify:** PigeonTweak viene eseguito all'interno dell'admin di Shopify e sulle pagine di stato dell'ordine e di ringraziamento. Shopify tratta i dati in conformità con la propria [Informativa sulla Privacy](https://www.shopify.com/legal/privacy). L'indirizzo di spedizione è memorizzato sull'ordine in Shopify.
- **Resend:** Consegna delle notifiche al merchant, come descritto sopra.
- **Hosting:** L'app è ospitata su Fly.io. Il suo database è un file SQLite su un volume cifrato negli Stati Uniti (Chicago).

## 5. Archiviazione, sicurezza e conservazione dei dati
I dati sono archiviati su un volume cifrato e trasmessi tramite connessioni cifrate (HTTPS). L'accesso è limitato allo sviluppatore. Lo sviluppatore adotta misure di sicurezza ragionevoli, ma nessun sistema è completamente sicuro e non è possibile garantire una sicurezza assoluta.

- **Uso attivo:** Impostazioni e sessioni vengono conservate finché l'app è installata. Gli altri dati vengono conservati per i periodi indicati nella Sezione 2.
- **Disinstallazione:** Quando disinstalli PigeonTweak, l'app elimina i dati che detiene per il tuo negozio. Il registro degli accessi viene eliminato quando Shopify invia `shop/redact`, circa 48 ore dopo.
- **Richieste sulla privacy di Shopify:** L'app gestisce i webhook obbligatori sulla privacy di Shopify (`customers/data_request`, `customers/redact` e `shop/redact`). Quando richiesto, fornisce o elimina i dati dei clienti che detiene.
- **Nessuna copia duratura degli indirizzi:** Fatta eccezione per i dati trattenuti temporaneamente descritti nella Sezione 2, l'app non conserva una copia dell'indirizzo di spedizione. L'indirizzo resta sull'ordine in Shopify, che controlli tu.
- **Email di supporto:** Conservate solo per il tempo necessario a gestire la tua richiesta, salvo che la legge richieda un periodo più lungo.

## 6. Incidenti di sicurezza
Lo sviluppatore è responsabile del contenimento di un incidente di sicurezza che esponga nome del cliente, indirizzo di spedizione, numero di telefono o dati dell'ordine trattati dall'app. Se lo sviluppatore viene a conoscenza di un tale incidente, lo contiene e avvisa Shopify all'indirizzo [security@shopify.com](mailto:security@shopify.com) entro 24 ore. I merchant interessati vengono avvisati come richiesto dalla legge applicabile.

## 7. Trasferimenti internazionali di dati
Lo sviluppatore e i fornitori di servizi sopra elencati possono trattare i dati in paesi diversi dal tuo, anche negli Stati Uniti e al di fuori dello Spazio Economico Europeo. In tal caso vengono applicate garanzie adeguate (come le Clausole Contrattuali Standard) come richiesto dalla legge applicabile.

## 8. Conformità e diritti
In conformità con il GDPR, il UK GDPR, il CCPA/CPRA e le altre leggi applicabili sulla privacy, gli interessati hanno il diritto di accedere, rettificare, cancellare, limitare o esportare i propri dati e di opporsi al loro trattamento.

- **Dati del tuo negozio:** Modifica le impostazioni nell'app in qualsiasi momento, oppure disinstalla l'app per eliminare i tuoi dati. Contatta lo sviluppatore per altre richieste.
- **Dati dei tuoi clienti:** Sei il titolare del trattamento dei dati degli ordini dei clienti. Un cliente deve contattare il tuo negozio in merito a un ordine. Puoi anche contattare lo sviluppatore all'indirizzo email indicato di seguito, indicando il dominio del negozio. Le richieste ricevono risposta entro 30 giorni.

PigeonTweak non vende né condivide informazioni personali e non adotta decisioni automatizzate che producano effetti giuridici o analogamente significativi. Hai inoltre il diritto di presentare un reclamo all'autorità locale per la protezione dei dati.

## 9. Privacy dei minori
PigeonTweak è uno strumento professionale per i merchant Shopify e non è rivolto ai minori. Lo sviluppatore non raccoglie consapevolmente informazioni personali da persone di età inferiore ai 16 anni, al di là dei dati di spedizione che un cliente invia su un ordine che il merchant già detiene.

## 10. Modifiche a questa informativa
Questa informativa può essere aggiornata di tanto in tanto. La data di "Ultimo aggiornamento" in alto indica la revisione più recente. Le modifiche significative saranno comunicate tramite l'app o via email.

## 11. Informazioni di contatto
Per qualsiasi domanda riguardante la tua privacy, puoi contattare lo sviluppatore all'indirizzo:<br>
**{{ site.email }}**
