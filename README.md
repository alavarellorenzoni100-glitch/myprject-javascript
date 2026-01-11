# Progetto TypeScript - Calcolatrice Area Cerchio e Gestione Spesa

Un progetto TypeScript che include una calcolatrice interattiva per calcolare l'area dei cerchi e un sistema per verificare gli sconti sulla spesa.

## 🚀 Funzionalità

- **Calcolo Area Cerchio**: Calcola l'area di uno o più cerchi dato il raggio
- **Gestione Spesa**: Verifica se una spesa supera la soglia per ottenere uno sconto del 10%
- **Interfaccia Web Interattiva**: Pagina HTML con interfaccia utente moderna e responsive

## 📁 Struttura del Progetto

```
progetti-typescript/
├── src/
│   ├── Index.ts          # File TypeScript principale con funzioni
│   ├── app.ts            # File TypeScript per l'interfaccia web
│   ├── area-cerchio.ts   # Modulo per il calcolo area cerchio
│   └── calcolatrice.ts   # Modulo calcolatrice
├── dist/                 # File JavaScript compilati (esclusi da git)
├── dist-browser/         # File JavaScript per browser (esclusi da git)
├── index.html            # Pagina web interattiva
├── tsconfig.json         # Configurazione TypeScript principale
├── tsconfig.browser.json # Configurazione TypeScript per browser
└── README.md             # Questo file
```

## 🛠️ Requisiti

- Node.js
- npm (Node Package Manager)
- TypeScript

## 📦 Installazione

### Installazione automatica

Esegui lo script di installazione:

```bash
chmod +x installa_ts.sh
./installa_ts.sh
```

### Installazione manuale

1. Installa TypeScript globalmente:
```bash
npm install -g typescript
```

2. Installa TypeScript e TSX per sviluppo:
```bash
npm install -g typescript tsx
```

## 🎯 Utilizzo

### Compilazione TypeScript

Compila tutti i file TypeScript:
```bash
tsc
```

Compila solo il file per browser:
```bash
tsc -p tsconfig.browser.json
```

### Esecuzione

#### Apri la pagina web

Apri semplicemente `index.html` nel tuo browser preferito:

```bash
xdg-open index.html
```

Oppure avvia un server HTTP locale:

```bash
python3 -m http.server 8000
```

Poi apri nel browser: `http://localhost:8000`

### Funzionalità della Pagina Web

1. **Calcolo Area Cerchio**
   - Inserisci i raggi di due cerchi
   - Clicca "Calcola Aree" per vedere i risultati
   - Visualizza il confronto tra le due aree

2. **Gestione Spesa**
   - Inserisci il totale della spesa
   - Clicca "Verifica Sconto" per vedere se hai diritto allo sconto del 10%
   - Visualizza il totale finale con sconto applicato

3. **Calcolo Automatico**
   - Clicca "Esegui Calcolo Automatico" per eseguire i calcoli con valori predefiniti
   - Raggio A: 15
   - Raggio B: 20
   - Spesa: €110

## 📝 Codice di Esempio

### Funzione Calcolo Area Cerchio

```typescript
function calcolaAreaCerchio(raggio: number): number {
    const pi: number = 3.14159;
    return pi * (raggio ** 2);
}
```

### Esempio di Utilizzo

```typescript
const raggio = 15;
const area = calcolaAreaCerchio(raggio);
console.log(`Area del cerchio: ${area.toFixed(2)}`);
```

## 🔧 Configurazione

Il progetto utilizza due configurazioni TypeScript:

- `tsconfig.json`: Configurazione principale per compilazione Node.js
- `tsconfig.browser.json`: Configurazione per compilazione browser (ES2020 modules)

## 📄 Licenza

Questo progetto è disponibile per uso educativo e personale.

## 👤 Autore

alavarellorenzoni100

## 🔗 Repository

[GitHub Repository](https://github.com/alavarellorenzoni100-glitch/myprject-javascript.git)
