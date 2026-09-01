# Panoramica CLI — @ares/jquery

## Stato

Questo modulo **non ha una CLI binaria** (`package.json` senza `bin`). È una libreria di parsing HTML importabile.

## Comandi (npm scripts)

| Comando | Scopo |
|---|---|
| `npm test` | Placeholder (nessun test definito, ritorna errore). |

## API runtime (import)

```js
import { parse, parseFile, parseUrl, parseCode } from "@ares/jquery";

// Parsing automatico (rileva URL, file o codice)
const result = await parse("https://example.com");
const result2 = await parse("./page.html");
const result3 = await parse("<html>...</html>");

// Parsing esplicito
const fileResult = await parseFile("./local.html");
const urlResult = await parseUrl("https://example.com");
const codeResult = await parseCode("<html>...</html>", { "content-type": "text/html" });

// Risultato: { window, $ (jQuery), headers }
const $ = result.$;
$("h1").text(); // queries jQuery sul DOM
```
