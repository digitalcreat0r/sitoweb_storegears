---
layout: document
title: Privacy Policy - GhostShelf
permalink: /it/policies/privacy-policy-ghostshelf.html
lang: it
back_url: /it/
back_text: Torna alla Home
---
# Privacy Policy - GhostShelf

*Ultimo aggiornamento: 23 ottobre 2026*

**GhostShelf** è un'applicazione per i merchant Shopify, sviluppata e gestita da **{{ site.author }}** ("lo sviluppatore"), operante come **{{ site.brand }}**. È progettata seguendo il principio di "Privacy by Design" (Privacy fin dalla progettazione): GhostShelf è rigorosamente **in sola lettura**, richiede solo gli accessi di cui ha bisogno e non modifica mai i tuoi prodotti, prezzi, giacenze o pubblicazioni. Questa informativa spiega quali dati l'app consulta, perché e come vengono trattati.

## 1. Titolare del Trattamento dei Dati
Per i dati di contatto e di supporto descritti in questa informativa, il titolare del trattamento è:

**{{ site.author }} ({{ site.brand }})**

Email: {{ site.email }}<br>
Sito web: {{ site.url }}

Per i dati del negozio che GhostShelf legge dal tuo negozio Shopify, il titolare del trattamento sei tu (il merchant), mentre lo sviluppatore agisce come responsabile del trattamento e tratta tali dati solo per fornire il servizio che hai installato.

## 2. Raccolta delle Informazioni
GhostShelf **non** raccoglie, memorizza o tratta informazioni personali sui tuoi clienti. Non legge nomi, indirizzi email, numeri di telefono né indirizzi di spedizione e di fatturazione dei clienti.

### Dati del Negozio Consultati tramite Shopify
Quando installi l'app, le concedi i seguenti permessi di accesso (scope):
- **`read_products`:** Utilizzato per leggere i prodotti attivi (titolo, handle, stato, tag, appartenenza alle collezioni, varianti, SKU e prezzi) così che l'app possa verificare se ciascun prodotto è ancora vendibile.
- **`read_inventory`:** Utilizzato per leggere i livelli di giacenza e le sedi di magazzino, così che l'app possa rilevare i prodotti esauriti o senza scorte in una sede che evade gli ordini online.
- **`read_publications`:** Utilizzato per leggere i canali di vendita su cui è pubblicato ciascun prodotto, così che l'app possa rilevare i prodotti non pubblicati nell'Online Store.
- **`read_orders` (facoltativo):** Richiesto solo se attivi l'impostazione degli Avvisi "avvisami solo se il prodotto è stato venduto negli ultimi 30 giorni". L'app legge solo il prodotto e la quantità delle righe degli ordini recenti, per sapere quali prodotti sono stati venduti di recente. Non legge informazioni sui clienti e non memorizza gli ordini.

L'app legge inoltre i dati di base del negozio: dominio, indirizzo email del negozio, valuta e fuso orario. L'email del negozio serve a suggerire un indirizzo predefinito per gli avvisi, mentre il fuso orario serve ad applicare le tue ore di silenzio.

### Dati Forniti dall'Utente nell'App
- **Destinazioni degli avvisi:** Un indirizzo email e fino a tre URL di webhook in ingresso di Slack, scelti da te, affinché l'app sappia dove inviare gli avvisi.
- **Impostazioni:** Le preferenze sulle regole, le esclusioni (prodotti, tag o collezioni che scegli di ignorare) e le ore di silenzio.

### Dati Generati dall'App
- **Stato dei prodotti e incidenti:** Un registro dei prodotti che al momento non rispettano una regola, di quando ogni problema è stato aperto o risolto e del motivo.
- **Registro degli avvisi:** Il canale, lo stato di consegna e l'orario di ciascun avviso inviato.
- **Registri tecnici:** Sessioni di autenticazione (dominio del negozio, token di accesso, scope concessi) e registri dei processi in background necessari per eseguire le scansioni e consegnare gli avvisi.

### Supporto e Feedback (Volontario)
Se contatti lo sviluppatore via email, puoi fornire volontariamente il tuo nome, il tuo indirizzo email e il dominio del tuo negozio. Queste informazioni vengono utilizzate esclusivamente per rispondere alla tua richiesta e risolvere problemi tecnici. Non vengono utilizzate per nessun altro scopo.

### Analisi, Pubblicità e Tracciamento
GhostShelf **non** utilizza strumenti di analisi, tracker pubblicitari né profilazione. Non vende né condivide i tuoi dati per finalità di marketing.

## 3. Come Vengono Consegnati gli Avvisi
Gli avvisi sono volutamente minimali. Contengono solo il numero di prodotti attivi non più vendibili e un invito ad aprire GhostShelf. Non includono nomi di prodotti, prezzi o dati dei clienti.
- **Email:** Inviata tramite **Resend** (resend.com), un fornitore di servizi di consegna email. Il tuo indirizzo email per gli avvisi e il testo dell'avviso vengono trattati da Resend solo per consegnare il messaggio. Consulta l'[Informativa sulla Privacy di Resend](https://resend.com/legal/privacy-policy).
- **Slack:** Pubblicato direttamente sull'URL del webhook in ingresso che fornisci. Slack tratta il messaggio in conformità con la propria [Informativa sulla Privacy](https://slack.com/trust/privacy/privacy-policy). Considera l'URL del webhook un segreto, poiché chiunque lo possieda può scrivere in quel canale.

## 4. Servizi di Terze Parti
- **Shopify:** GhostShelf viene eseguito all'interno dell'admin di Shopify e utilizza la Shopify Admin API. Shopify tratta i dati in conformità con la propria [Informativa sulla Privacy](https://www.shopify.com/legal/privacy).
- **Resend:** Consegna degli avvisi via email, come descritto sopra.
- **Slack:** Consegna degli avvisi su Slack, come descritto sopra (solo se lo configuri).
- **Fornitori di hosting e database:** L'app e il suo database sono ospitati presso fornitori di infrastruttura cloud gestita, che conservano i dati per conto dello sviluppatore nel rispetto di adeguati obblighi di sicurezza e riservatezza.

## 5. Archiviazione, Sicurezza e Conservazione dei Dati
I dati dell'app sono archiviati in un database PostgreSQL gestito. I dati vengono trasmessi tramite connessioni cifrate (HTTPS) e l'accesso è limitato allo sviluppatore.
- **Uso attivo:** I dati vengono conservati finché l'app è installata nel tuo negozio, affinché avvisi e cronologia continuino a funzionare.
- **Disinstallazione:** Quando disinstalli GhostShelf, l'app riceve la notifica `app/uninstalled` di Shopify ed elimina i dati che detiene per il tuo negozio: impostazioni, esclusioni, stato dei prodotti, incidenti, destinazioni degli avvisi, registri degli avvisi, processi e sessioni.
- **Richieste di conformità Shopify:** L'app gestisce i webhook obbligatori sulla privacy di Shopify. Con `shop/redact`, tutti i dati residui del negozio vengono eliminati. Poiché GhostShelf non memorizza dati personali dei clienti, le richieste `customers/data_request` e `customers/redact` non hanno dati dei clienti da restituire o eliminare.
- **Email di supporto:** Conservate solo per il tempo necessario a gestire la tua richiesta e poi eliminate, salvo che la legge richieda un periodo più lungo.

## 6. Trasferimenti Internazionali di Dati
Lo sviluppatore e i fornitori di servizi sopra elencati possono trattare i dati in paesi diversi dal tuo, anche al di fuori dello Spazio Economico Europeo. In tal caso vengono applicate garanzie adeguate (come le Clausole Contrattuali Standard) come richiesto dalla legge applicabile.

## 7. Conformità e Diritti dell'Utente
In conformità con il GDPR, il UK GDPR, il CCPA/CPRA e le altre leggi applicabili sulla privacy, hai il diritto di accedere, rettificare, cancellare, limitare o esportare i tuoi dati e di opporti al loro trattamento. Puoi esercitare tali diritti come segue:
- **Eliminare i dati:** Rimuovi in qualsiasi momento le destinazioni degli avvisi e le esclusioni nell'app, oppure disinstalla l'app per eliminare tutti i dati del negozio (vedi Sezione 5).
- **Altre richieste:** Contatta lo sviluppatore all'indirizzo email indicato di seguito. Le richieste ricevono risposta entro 30 giorni.

GhostShelf non vende né condivide informazioni personali e non adotta decisioni automatizzate che producano effetti giuridici o analogamente significativi su di te. Hai inoltre il diritto di presentare un reclamo all'autorità locale per la protezione dei dati.

## 8. Privacy dei Minori
GhostShelf è uno strumento professionale per i merchant Shopify e non è rivolto ai minori. Lo sviluppatore non raccoglie consapevolmente informazioni personali da persone di età inferiore ai 16 anni.

## 9. Modifiche a Questa Informativa
Questa informativa può essere aggiornata di tanto in tanto, ad esempio quando cambiano le funzionalità dell'app. La data di "Ultimo aggiornamento" in alto indica la revisione più recente. Le modifiche significative saranno comunicate tramite l'app o via email.

## 10. Informazioni di Contatto
Per qualsiasi domanda riguardante la tua privacy, puoi contattare lo sviluppatore all'indirizzo:<br>
**{{ site.email }}**
