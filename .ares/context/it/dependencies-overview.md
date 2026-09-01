# Dipendenze — @ares/jquery

## Dipendenze @ares/* usate

Nessuna dipendenza runtime `@ares/*`. Il modulo è completamente autonomo.

## Dipendenze @ares/* (dev)

| Modulo | Perché |
|---|---|
| `@ares/scd` | Strumenti SCD per analisi/generazione documentazione. |

## Dipendenze esterne rilevanti

- `jsdom` — implementazione DOM per Node.js (usata per creare l'ambiente `window` e il document).
- `jquery` — libreria jQuery caricata sul DOM JSDOM per il querying CSS/xpath.
- `axios` — client HTTP per il download di pagine web da URL.
- `fs` — modulo Node.js nativo per la lettura di file HTML locali.
- `mime` — rilevamento del MIME type dei file per l'header `content-type`.

## Chi dipende da questo modulo

Nessun altro modulo aReS dichiara `@ares/jquery` come dipendenza nei relativi `package.json` (ad oggi). Il modulo è progettato per essere usato dai moduli applicativi che necessitano di parsing HTML/DOM.
