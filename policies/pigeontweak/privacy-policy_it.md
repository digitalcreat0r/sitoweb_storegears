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

**PigeonTweak** è un'applicazione per i merchant Shopify, sviluppata e gestita da **{{ site.author }}** ("lo sviluppatore"), operante come **{{ site.brand }}**. Consente a un cliente autenticato di correggere l'indirizzo di spedizione di un ordine dalla pagina di stato dell'ordine o dalla pagina di ringraziamento, finché la tua finestra di modifica è ancora aperta e l'ordine può ancora essere modificato. Il paese sull'indirizzo resta lo stesso. Questa informativa spiega quali dati l'app consulta, perché e per quanto tempo vengono conservati.

## 1. Chi è responsabile dei dati
Per i dati del negozio e per i dati dei clienti che PigeonTweak legge o aggiorna nel tuo negozio Shopify (nome, indirizzo di spedizione e telefono di un cliente su un ordine), il titolare del trattamento sei tu (il merchant). Lo sviluppatore agisce come responsabile del trattamento e tratta tali dati solo per fornire il servizio che hai installato.

Per i dati di contatto e di supporto (ad esempio quando ci scrivi via email), il titolare del trattamento è **{{ site.author }} ({{ site.brand }})**, {{ site.email }}.

## 2. Dati che l'app consulta
PigeonTweak tratta i dati dei clienti solo affinché un cliente titolare di un ordine possa correggere l'indirizzo di spedizione, e affinché tu possa essere informato che l'indirizzo è cambiato. Non costruisce un elenco di clienti e non legge gli indirizzi email dei clienti.

Quando installi l'app, le concedi questi permessi di accesso (scope):

- **`read_orders`:** Legge l'ordine che il cliente sta visualizzando: nome e id dell'ordine, stato, data di creazione, stato di evasione, totale e indirizzo di spedizione attuale (nome, azienda, via, città, provincia, codice postale, paese, telefono).
- **`write_orders`:** Salva sull'ordine il nuovo indirizzo di spedizione. L'app non modifica le righe dell'ordine, gli sconti o i prodotti.
- **`read_customers`:** Conferma che il cliente autenticato sia il titolare dell'ordine. L'app non legge indirizzi email, preferenze di marketing né altri dati del profilo.
- **`read_merchant_managed_fulfillment_orders` e `read_third_party_fulfillment_orders`:** Verificano se una richiesta di evasione è già stata inviata. Se lo è, l'indirizzo non può più essere modificato.
- **`write_app_proxy`:** Permette al modulo dell'ordine di chiamare l'app attraverso il dominio del tuo negozio.

L'app legge inoltre il nome del negozio, il dominio, l'indirizzo email del negozio e il fuso orario. L'email del negozio è l'indirizzo a cui vengono inviate le notifiche al merchant, mentre il fuso orario serve per le tue ore di silenzio.

Il cliente autenticato invia il nuovo indirizzo (nome, azienda, via, città, provincia o stato, codice postale e telefono, in base ai campi che abiliti). Tu fornisci le impostazioni nell'app: se le correzioni sono attive, la finestra di modifica, i campi del modulo e le preferenze su email e ore di silenzio.

## 3. Dati che l'app conserva e per quanto tempo
- **Impostazioni e sessioni:** Conservate finché l'app è installata. Le sessioni contengono il dominio del negozio, le credenziali di accesso e gli scope concessi. Per una sessione online dello staff contengono anche id utente Shopify, nome ed email del membro dello staff.
- **Conteggio delle correzioni:** Un conteggio giornaliero delle correzioni riuscite (dominio del negozio, data, numero). Non contiene ordine, nome, indirizzo o telefono. Eliminato dopo circa 30 giorni.
- **Dati trattenuti temporaneamente:** Se una correzione cambia il totale dell'ordine, l'app conserva per alcuni minuti l'indirizzo precedente e la notifica (compresi nome e telefono), così che il cliente possa annullare la modifica. Le notifiche ritardate dalle tue ore di silenzio vengono conservate fino all'invio. Eliminati una volta gestiti, e comunque entro 90 giorni.
- **Registro degli accessi:** Quando nome, indirizzo o telefono di un cliente vengono letti, salvati, esportati o eliminati, l'app registra dominio del negozio, id dell'ordine, azione e id del cliente. Non memorizza nome, indirizzo o telefono. Eliminato dopo 90 giorni.
- **Email di supporto:** Se ci contatti, conserviamo nome, email e dominio del negozio solo per il tempo necessario a risponderti, salvo che la legge richieda un periodo più lungo.

Fatta eccezione per i dati trattenuti temporaneamente, l'app non conserva una copia dell'indirizzo di spedizione. L'indirizzo resta sull'ordine in Shopify, che controlli tu.

**Disinstallazione e richieste sulla privacy:** Quando disinstalli PigeonTweak, l'app elimina i dati che detiene per il tuo negozio. Il registro degli accessi viene eliminato quando Shopify invia `shop/redact`, circa 48 ore dopo. L'app gestisce inoltre i webhook obbligatori sulla privacy di Shopify (`customers/data_request`, `customers/redact` e `shop/redact`).

## 4. Notifiche al merchant e terze parti
Se le notifiche al merchant sono attive, l'app invia un'email all'indirizzo email del tuo negozio quando un indirizzo cambia. Il messaggio include il nome dell'ordine, l'indirizzo precedente e quello nuovo (compresi nome e telefono) e, se il totale dell'ordine è cambiato, il totale precedente e quello nuovo.

- **Shopify:** PigeonTweak viene eseguito all'interno dell'admin di Shopify e sulle pagine di stato dell'ordine e di ringraziamento. Shopify tratta i dati secondo la propria [Informativa sulla Privacy](https://www.shopify.com/legal/privacy).
- **Resend:** Consegna solo le notifiche al merchant. Consulta l'[Informativa sulla Privacy di Resend](https://resend.com/legal/privacy-policy).
- **Hosting:** L'app è ospitata su Fly.io. Il suo database è un file SQLite su un volume cifrato negli Stati Uniti (Chicago).

PigeonTweak non utilizza strumenti di analisi di terze parti, tracker pubblicitari né profilazione. Non vende né condivide i tuoi dati, né quelli dei tuoi clienti, per finalità di marketing e non adotta decisioni automatizzate con effetti giuridici.

## 5. Sicurezza e trasferimenti internazionali
I dati sono archiviati su un volume cifrato, trasmessi tramite HTTPS e accessibili solo allo sviluppatore. Nessun sistema è completamente sicuro, quindi non è possibile garantire una sicurezza assoluta. Se un incidente di sicurezza espone nome, indirizzo, telefono o dati dell'ordine di un cliente, lo sviluppatore lo contiene, avvisa Shopify all'indirizzo [security@shopify.com](mailto:security@shopify.com) entro 24 ore e avvisa i merchant interessati come richiesto dalla legge.

I dati possono essere trattati in paesi diversi dal tuo, anche negli Stati Uniti e al di fuori dello Spazio Economico Europeo. In tal caso vengono applicate garanzie adeguate (come le Clausole Contrattuali Standard) come richiesto dalla legge.

## 6. I tuoi diritti
In base al GDPR, al UK GDPR, al CCPA/CPRA e alle altre leggi applicabili, hai il diritto di accedere, rettificare, cancellare, limitare o esportare i tuoi dati e di opporti al loro trattamento. Puoi anche presentare un reclamo all'autorità locale per la protezione dei dati.

- **Dati del tuo negozio:** Modifica le impostazioni nell'app in qualsiasi momento, oppure disinstalla l'app per eliminare i tuoi dati. Contattaci per altre richieste.
- **Dati dei tuoi clienti:** Sei il titolare del trattamento, quindi un cliente deve contattare il tuo negozio in merito a un ordine. Puoi anche scriverci indicando il dominio del negozio.

Rispondiamo alle richieste entro 30 giorni. PigeonTweak è uno strumento professionale e non è rivolto ai minori.

## 7. Modifiche e contatti
Questa informativa può essere aggiornata di tanto in tanto. La data di "Ultimo aggiornamento" indica la revisione più recente. Le modifiche significative saranno comunicate tramite l'app o via email.

Domande sulla tua privacy: **{{ site.email }}**
