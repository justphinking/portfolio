# ulisse-portfolio

Sito portfolio personale con assistente AI.

## Struttura

```
ulisse-portfolio/
├── api/
│   └── chat.js          # Funzione serverless (proxy API Anthropic)
├── public/
│   ├── index.html       # Interfaccia chat
│   └── img/             # Directory immagini
│       ├── ritratto.jpg
│       ├── coro.jpg
│       ├── ep.jpg
│       └── motion.jpg
├── vercel.json          # Configurazione Vercel
└── README.md
```

## Deploy su Vercel

### 1. GitHub
- Crea un repository su github.com (es. `ulisse-portfolio`)
- Carica tutti i file del progetto

### 2. Vercel
- Vai su vercel.com → "Add New Project"
- Collega il repository GitHub
- Nella sezione "Environment Variables" aggiungi:
  - Name: `ANTHROPIC_API_KEY`
  - Value: la tua chiave API da platform.anthropic.com
- Clicca "Deploy"

### 3. Immagini
Carica nella cartella `public/img/` le seguenti immagini:
- `ritratto.jpg` — foto di Ulisse
- `coro.jpg` — foto del Coro del Pigneto
- `ep.jpg` — copertina EP "Musica da camera"
- `motion.jpg` — esempio di motion graphics

Le immagini vengono mostrate inline nella chat quando pertinenti.

## Chiave API Anthropic
Ottienila su: https://platform.anthropic.com/api-keys
Costo stimato: 2-5€/mese con traffico normale.
