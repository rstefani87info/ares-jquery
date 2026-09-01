# Documentazione @ares/jquery

## Scopo

JQuery for cheerio parsing

## Installazione

```bash
yarn add @ares/jquery
```

In un monorepo Yarn Workspaces:

```bash
yarn workspace <app> add @ares/jquery
```

## Quickstart

Esempio minimale:

```js
import * as mod from "@ares/jquery";
```

## API pubbliche (exports)

Questa sezione documenta la superficie pubblica reale a livello di entrypoint e simboli principali.

Entrypoint root:

- `@ares/jquery`

File principali nel root del package (indicativi):

- `index.js`

Export individuati in `index.*`:

- `parse`
- `parseCode`
- `parseFile`
- `parseUrl`

## Configurazione (appSetup / config / policies)

Questo modulo può leggere configurazioni da `appSetup`, `config` o `policies` a seconda del tipo. Documenta qui le chiavi effettivamente consumate quando stabilizzi il contract.

## Test

Esecuzione test del modulo (se presenti):

```bash
yarn workspace @ares/jquery test
```

## Note

- Questo documento è mantenuto in parallelo ai ticket del modulo.
