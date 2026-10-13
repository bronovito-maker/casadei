# Refactor UI/UX — Ristrutturazioni Casadei

## Intervento

- Stack conservato: HTML, CSS e JavaScript statici, una sola pagina.
- Marchio testuale «Casadei Ristrutturazioni»; palette mantenuta, fondi caldi e CTA rosse coerenti.
- Tipografia sans-serif di sistema, testo principale 17–18 px e scala responsive condivisa.
- Hero con servizio e zona, immagine illustrativa fornita dal cliente, preventivo e accesso ai lavori. La parola «Rimini» usa un serif corsivo.
- Servizi su griglia aperta; progetti prima/dopo; metodo; impresa; recensioni; comuni; FAQ e contatti.
- Menu mobile a disclosure, supporto tastiera, Escape e chiusura quando il focus esce.
- Contatti diretti WhatsApp, telefono ed email. Nessun modulo era presente nel sito iniziale.
- Indirizzo e collegamento alla mappa rimossi; indirizzo eliminato anche dai dati strutturati.
- Titolo SEO, descrizione, canonical, Open Graph, dati dell'impresa e comuni serviti conservati.
- Archivio di pubblicazione escluso dal controllo versione; immagini complessivamente circa 1,30 MB.

## Verifiche eseguite

| Larghezza | Overflow orizzontale | Testi tagliati |
| --- | --- | --- |
| 360 px | Nessuno | Nessuno |
| 390 px | Nessuno | Nessuno |
| 768 px | Nessuno | Nessuno |
| 1440 px | Nessuno | Nessuno |

- Ispezione visiva dell'apertura desktop e mobile e della sezione servizi su tablet.
- Link per saltare al contenuto e focus visibile: outline di 3 px.
- Menu aperto da tastiera; Tab raggiunge le voci; Escape chiude e restituisce focus al pulsante.
- Il menu si chiude quando il focus passa al contenuto della pagina.
- Link ai lavori e ai servizi verificati: sezione visibile sotto l'intestazione sticky.
- FAQ aperta e richiusa con Enter.
- Destinazioni WhatsApp, telefono ed email verificate nel DOM; nessuna chiamata o messaggio inviato.
- Contrasto dei testi renderizzati: minimo circa 5,01:1; nessuna combinazione sotto la soglia applicabile.
- Asset e ancore verificati; JSON-LD sintatticamente valido; un solo H1; nessuna via o mappa residua nella pagina.
- Controllo sintattico JavaScript superato (`node --check`). Lo stack statico non prevede un comando di build.
- Movimento ridotto gestito nei CSS: scroll immediato e transizioni disattivate.

## Materiali ancora utili

Le immagini fornite mostrano in gran parte fasi di cantiere. La hero valorizza dettagli realmente posati, e le fotografie dei progetti indicano lo stato della lavorazione. Per una presentazione più forte servono foto originali ampie, ben illuminate e senza scritte di un bagno e di un appartamento completamente finiti. I casi di lavoro conservano le fotografie originali. La nuova immagine fornita dal cliente è usata solo nella hero, con didascalia illustrativa.

## Anteprime

- `anteprime/desktop-1440.jpg`
- `anteprime/mobile-390.jpg`

## Pubblicazione

Refactor pubblicato con successo sul sito esistente, preservando l'accesso pubblico:
https://ristrutturazioni-casadei.bronovito.chatgpt.site/

## Modifiche dai commenti del browser

Immagine allegata sostituita nella hero e ottimizzata in due risoluzioni (circa 89 KB e 271 KB); marchio testuale al posto del logo illustrato in header e footer; serif corsivo sulla parola «Rimini»; favicon CR. Verificate anche le larghezze 355, 360, 390, 768 e 1440 px: nessun overflow o testo tagliato.

## Ruolo di Nicholas

Testi di hero, servizi, metodo, impresa e FAQ aggiornati: Nicholas è l’artigiano che esegue i lavori in prima persona ed è anche il referente del cliente. Gli altri professionisti intervengono a supporto nelle lavorazioni specialistiche e nelle ristrutturazioni complete. Anteprima a 355 px: nessun overflow o testo tagliato.

## Revisione dei testi — 14 ottobre 2026

- Hero: Nicholas esegue le opere edili e organizza il cantiere; il cliente ha un unico referente anche nelle ristrutturazioni complete.
- Titoli dei servizi, lavori e zona operativa resi descrittivi. Ridotte le ripetizioni e concentrati nel metodo i dettagli sul coordinamento e sugli impianti.
- CTA della hero con indicazione visibile «Scrivici su WhatsApp»; destinazione invariata.
- Nessuna località o promessa aggiunta ai singoli lavori senza documentazione. Recensioni, contatti, dati fiscali e metadati preservati.
- Verifica in browser a 360, 390, 768 e 1440 px: nessun overflow. Menu mobile apre e chiude con Escape.
- Controlli `git diff --check` e `node --check dist/app.js` superati. Sito statico: nessuna compilazione richiesta.
