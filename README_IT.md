# Eliza 🤖

<div align="center">
  <img src="./docs/static/img/eliza_banner.jpg" alt="Eliza Banner" width="100%" />
</div>

<div align="center">

📖 [Documentazione](https://elizaos.github.io/eliza/) | 🎯 [Esempi](https://github.com/thejoven/awesome-eliza)

</div>

## 🌍 Traduzioni del README

[中文说明](./README_CN.md) | [日本語の説明](./README_JA.md) | [한국어 설명](./README_KOR.md) | [Français](./README_FR.md) | [Português](./README_PTBR.md) | [Türkçe](./README_TR.md) | [Русский](./README_RU.md) | [Español](./README_ES.md) | [Italiano](./README_IT.md) | [ไทย](./README_TH.md) | [Deutsch](./README_DE.md) | [Tiếng Việt](./README_VI.md) | [עִברִית](https://github.com/elizaos/Elisa/blob/main/README_HE.md)

## ✨ Caratteristiche

- 🛠️ Connettori completi per Discord, Twitter e Telegram
- 🔗 Supporto per ogni modello (Llama, Grok, OpenAI, Anthropic, ecc.)
- 👥 Supporto multi-agente e per stanze
- 📚 Ingestione e interazione facile con i tuoi documenti
- 💾 Memoria recuperabile e archivio documenti
- 🚀 Altamente estensibile - crea le tue azioni e clienti
- ☁️ Supporta molti modelli (Llama locale, OpenAI, Anthropic, Groq, ecc.)
- 📦 Funziona subito!

## Video Tutorial

[AI Agent Dev School](https://www.youtube.com/watch?v=ArptLpQiKfI&list=PLx5pnFXdPTRzWla0RaOxALTSTnVq53fKL)

## 🎯 Casi d'Uso

- 🤖 Chatbot
- 🕵️ Agenti Autonomi
- 📈 Gestione dei Processi Aziendali
- 🎮 NPC nei Videogiochi
- 🧠 Trading

## 🚀 Avvio Rapido

### Prerequisiti

- [Python 2.7+](https://www.python.org/downloads/)
- [Node.js 23+](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- [pnpm](https://pnpm.io/installation)

> **Nota per gli Utenti Windows:** È richiesto [WSL 2](https://learn.microsoft.com/en-us/windows/wsl/install-manual).

### Usa lo Starter (Consigliato)

```bash
git clone https://github.com/elizaos/eliza-starter.git
cd eliza-starter
cp .env.example .env
pnpm i && pnpm build && pnpm start
```

Poi leggi la [Documentazione](https://elizaos.github.io/eliza/) per imparare come personalizzare il tuo Eliza.

### Avvia Eliza Manualmente (Consigliato solo se sai cosa stai facendo)

```bash
# Clona il repository
git clone https://github.com/elizaos/eliza.git

# Passa all'ultima release
# Questo progetto si evolve rapidamente, quindi consigliamo di passare all'ultima release
git checkout $(git describe --tags --abbrev=0)
```

### Avvia Eliza con Gitpod

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/elizaos/eliza/tree/main)

### Modifica il file .env

Copia .env.example in .env e inserisci i valori appropriati.

```
cp .env.example .env
```

Nota: .env è opzionale. Se hai intenzione di eseguire più agenti distinti, puoi passare i segreti attraverso il JSON del personaggio.

### Avvio Automatico di Eliza

Questo eseguirà tutto per impostare il progetto e avviare il bot con il personaggio predefinito.

```bash
sh scripts/start.sh
```

### Modifica il file del personaggio

1. Apri `packages/core/src/defaultCharacter.ts` per modificare il personaggio predefinito. Decommenta e modifica.

2. Per caricare personaggi personalizzati:
    - Usa `pnpm start --characters="path/to/your/character.json"`
    - Più file di personaggi possono essere caricati contemporaneamente
3. Connettiti con X (Twitter)
    - cambia `"clients": []` in `"clients": ["twitter"]` nel file del personaggio per connetterti con X

### Avvia Eliza Manualmente

```bash
pnpm i
pnpm build
pnpm start

# Il progetto si evolve rapidamente, a volte è necessario pulire il progetto se ci si ritorna
pnpm clean
```

#### Requisiti Aggiuntivi

Potrebbe essere necessario installare Sharp. Se vedi un errore all'avvio, prova a installarlo con il seguente comando:

```
pnpm install --include=optional sharp
```

### Comunità & contatti

- [GitHub Issues](https://github.com/elizaos/eliza/issues). Ideale per: bug che incontri usando Eliza e proposte di funzionalità.
- [Discord](https://discord.gg/ai16z). Ideale per: condividere le tue applicazioni e interagire con la comunità.

## Contributori

<a href="https://github.com/elizaos/eliza/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=elizaos/eliza" />
</a>

## Storico delle Stelle

[![Star History Chart](https://api.star-history.com/svg?repos=elizaos/eliza&type=Date)](https://star-history.com/#elizaos/eliza&Date)