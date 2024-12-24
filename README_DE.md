# Eliza 🤖

<div align="center">
  <img src="./docs/static/img/eliza_banner.jpg" alt="Eliza Banner" width="100%" />
</div>

<div align="center">

📖 [Dokumentation](https://elizaos.github.io/eliza/) | 🎯 [Beispiele](https://github.com/thejoven/awesome-eliza)

</div>

## 🌍 README Übersetzungen

[中文说明](./README_CN.md) | [日本語の説明](./README_JA.md) | [한국어 설명](./README_KOR.md) | [Français](./README_FR.md) | [Português](./README_PTBR.md) | [Türkçe](./README_TR.md) | [Русский](./README_RU.md) | [Español](./README_ES.md) | [Italiano](./README_IT.md) | [ไทย](./README_TH.md) | [Deutsch](./README_DE.md) | [Tiếng Việt](./README_VI.md) | [עִברִית](https://github.com/elizaos/Elisa/blob/main/README_HE.md)

## ✨ Funktionen

- 🛠️ Voll ausgestattete Discord-, Twitter- und Telegram-Konnektoren
- 🔗 Unterstützung für jedes Modell (Llama, Grok, OpenAI, Anthropic, etc.)
- 👥 Unterstützung für mehrere Agenten und Räume
- 📚 Einfaches Einlesen und Interagieren mit Ihren Dokumenten
- 💾 Abrufbarer Speicher und Dokumentenspeicher
- 🚀 Hochgradig erweiterbar - Erstellen Sie Ihre eigenen Aktionen und Clients
- ☁️ Unterstützt viele Modelle (lokales Llama, OpenAI, Anthropic, Groq, etc.)
- 📦 Funktioniert einfach!

## Video-Tutorials

[AI Agent Dev School](https://www.youtube.com/watch?v=ArptLpQiKfI&list=PLx5pnFXdPTRzWla0RaOxALTSTnVq53fKL)

## 🎯 Anwendungsfälle

- 🤖 Chatbots
- 🕵️ Autonome Agenten
- 📈 Geschäftsprozessabwicklung
- 🎮 Videospiel-NPCs
- 🧠 Handel

## 🚀 Schnellstart

### Voraussetzungen

- [Python 2.7+](https://www.python.org/downloads/)
- [Node.js 23+](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- [pnpm](https://pnpm.io/installation)

> **Hinweis für Windows-Nutzer:** [WSL 2](https://learn.microsoft.com/en-us/windows/wsl/install-manual) ist erforderlich.

### Verwenden Sie den Starter (Empfohlen)

```bash
git clone https://github.com/elizaos/eliza-starter.git
cd eliza-starter
cp .env.example .env
pnpm i && pnpm build && pnpm start
```

Lesen Sie dann die [Dokumentation](https://elizaos.github.io/eliza/), um zu erfahren, wie Sie Ihre Eliza anpassen können.

### Eliza manuell starten (Nur empfohlen, wenn Sie wissen, was Sie tun)

```bash
# Repository klonen
git clone https://github.com/elizaos/eliza.git

# Auf den neuesten Release wechseln
# Dieses Projekt entwickelt sich schnell weiter, daher empfehlen wir, den neuesten Release zu verwenden
git checkout $(git describe --tags --abbrev=0)
```

### Eliza mit Gitpod starten

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/elizaos/eliza/tree/main)

### Bearbeiten Sie die .env-Datei

Kopieren Sie .env.example zu .env und füllen Sie die entsprechenden Werte aus.

```
cp .env.example .env
```

Hinweis: .env ist optional. Wenn Sie planen, mehrere unterschiedliche Agenten zu betreiben, können Sie Geheimnisse über die Charakter-JSON übergeben.

### Eliza automatisch starten

Dies wird alles ausführen, um das Projekt einzurichten und den Bot mit dem Standardcharakter zu starten.

```bash
sh scripts/start.sh
```

### Bearbeiten Sie die Charakterdatei

1. Öffnen Sie `packages/core/src/defaultCharacter.ts`, um den Standardcharakter zu ändern. Kommentieren Sie aus und bearbeiten Sie.

2. Um benutzerdefinierte Charaktere zu laden:
    - Verwenden Sie `pnpm start --characters="path/to/your/character.json"`
    - Mehrere Charakterdateien können gleichzeitig geladen werden
3. Verbindung mit X (Twitter)
    - Ändern Sie `"clients": []` zu `"clients": ["twitter"]` in der Charakterdatei, um eine Verbindung mit X herzustellen

### Eliza manuell starten

```bash
pnpm i
pnpm build
pnpm start

# Das Projekt entwickelt sich schnell weiter, manchmal müssen Sie das Projekt bereinigen, wenn Sie zurückkehren
pnpm clean
```

#### Zusätzliche Anforderungen

Möglicherweise müssen Sie Sharp installieren. Wenn beim Starten ein Fehler auftritt, versuchen Sie, es mit dem folgenden Befehl zu installieren:

```
pnpm install --include=optional sharp
```

### Community & Kontakt

- [GitHub Issues](https://github.com/elizaos/eliza/issues). Am besten geeignet für: Fehler, die Sie bei der Verwendung von Eliza feststellen, und Funktionsvorschläge.
- [Discord](https://discord.gg/ai16z). Am besten geeignet für: Teilen Ihrer Anwendungen und Austausch mit der Community.

## Mitwirkende

<a href="https://github.com/elizaos/eliza/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=elizaos/eliza" />
</a>

## Sternverlauf

[![Star History Chart](https://api.star-history.com/svg?repos=elizaos/eliza&type=Date)](https://star-history.com/#elizaos/eliza&Date)