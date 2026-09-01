# Stili di sviluppo applicati — @ares/jquery

## Standard di programmazione

- Modulo **ESM** (`"type": "module"`) con entrypoint `index.js`.
- Uso di JSDOM come runtime DOM e jQuery come libreria DOM per il querying.
- Nessuno strumento di build/transpile: JS nativo ESM.
- Import di moduli Node.js nativi (`fs`) e librerie esterne (`axios`, `jsdom`, `jquery`, `mime`).

## Contratto directory / file

```text
jquery/
├─ index.js        # MANUALE  — intera implementazione parsing HTML/jQuery
├─ package.json    # MANUALE
├─ README.md       # MANUALE
├─ .gitignore      # MANUALE
├─ .git/           # GENERATO (locale)
└─ .ares/
   ├─ context/     # MANUALE   — doc di contesto (prodotto)
   ├─ docs/{en,it} # MANUALE   — documentazione
   └─ tasks/       # MANUALE   — task canonici
```

## Generato automaticamente vs Manuale

### Generato automaticamente (non committare)

- `.git/` (locale).

### Manuale (scritto a mano, NON rigenerare/sovrascrivere)

- `index.js` (l'intero contenuto del modulo da conservare).
- `package.json`, `README.md`, `.gitignore`.
- Tutti i file dentro `.ares/` (context, docs, tasks).

Nessuna directory di build/dist; il modulo è una libreria pura importabile.
