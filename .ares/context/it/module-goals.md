# Obiettivi del modulo @ares/jquery

## Introduzione

`@ares/jquery` è descritto in `package.json` come "JQuery for cheerio parsing". È un modulo ESM con entrypoint `index.js` che fornisce funzionalità di parsing HTML/XML con supporto jQuery tramite JSDOM e jsdom.

Modulo pensato per analisi di pagine web, file HTML e codice sorgente, con estrazione di meta tag e headers.

## Obiettivi principali

- Analizzare HTML da URL, file locali o stringhe di codice.
- Fornire un ambiente jQuery (`$`) per il querying del DOM tramite JSDOM.
- Estrarre meta tag e headers dai documenti HTML analizzati.
- Supportare il rilevamento automatico del tipo di input (URL, file, codice).

## Responsabilità

- `parse(htmlOrUrlOrPath)` — parsing automatico che rileva se l'input è un file locale, un URL o codice HTML.
- `parseFile(file)` — legge e analizza un file HTML locale.
- `parseUrl(url)` — scarica e analizza una pagina web tramite HTTP.
- `parseCode(code, headers)` — analizza una stringa HTML e restituisce oggetto con `window`, `$` (jQuery) e headers estratti.

## Cosa NON fa

- Non ha CLI binaria (`package.json` senza `bin`).
- Non gestisce rendering lato server completo (solo parsing DOM).
- Non implementa crawling/web scraping avanzato: è un modulo di parsing base.
