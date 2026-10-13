# Casadei Ristrutturazioni

Landing page per **Casadei Nicholas**, artigiano che realizza ristrutturazioni complete, bagni, pavimenti, rivestimenti, tinteggiature e opere in cartongesso a Rimini, Riccione, Misano Adriatico e Cattolica.

[Sito pubblicato](https://ristrutturazioni-casadei.bronovito.chatgpt.site/)

## Struttura

- `dist/index.html`: pagina, contenuti, metadati SEO e dati strutturati.
- `dist/styles.css`: stili condivisi e layout responsive.
- `dist/app.js`: menu mobile e interazioni accessibili.
- `dist/assets/`: immagini ottimizzate usate dal sito.
- `docs/`: analisi dei contenuti, piano del sito e resoconto delle verifiche.
- `source-materials/`: immagini originali fornite per il progetto.
- `.openai/hosting.json`: configurazione del sito esistente su Sites.

## Avvio locale

Il sito usa HTML, CSS e JavaScript statici. Non richiede dipendenze npm o una compilazione.

Dalla cartella del repository:

```sh
python3 -m http.server 4173 --directory dist --bind 127.0.0.1
```

Aprire [http://127.0.0.1:4173](http://127.0.0.1:4173).

Per controllare la sintassi JavaScript:

```sh
node --check dist/app.js
```

## Contenuti e immagini

Nicholas esegue i lavori in prima persona; nelle lavorazioni complesse e nelle ristrutturazioni complete si affianca a professionisti specializzati. I contatti principali sono WhatsApp, telefono ed email. Non è pubblicata una sede fisica.

L’immagine della hero è illustrativa ed è stata fornita per il progetto. Le fotografie nella sezione dei lavori documentano gli interventi Casadei; le didascalie distinguono le fasi di cantiere dai risultati della posa. Le recensioni riportano estratti autentici forniti dal cliente.

## Pubblicazione

Il sito è attualmente ospitato con Sites. Questo repository conserva il codice, gli asset e la documentazione: il push su GitHub, da solo, non aggiorna automaticamente il sito pubblicato. La cartella `dist/` può essere servita da un hosting statico; in caso di cambio dominio, aggiornare canonical e URL assoluti nei metadati e nei dati strutturati.

Gli archivi di pubblicazione e i file locali temporanei sono esclusi dal progetto tramite `.gitignore`.
