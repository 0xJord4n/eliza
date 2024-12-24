# Eliza 🤖

<div align="center">
  <img src="./docs/static/img/eliza_banner.jpg" alt="Bannière Eliza" width="100%" />
</div>

<div align="center">

📖 [Documentation](https://elizaos.github.io/eliza/) | 🎯 [Exemples](https://github.com/thejoven/awesome-eliza)

</div>

## 🌍 Traductions du README

[中文说明](./README_CN.md) | [日本語の説明](./README_JA.md) | [한국어 설명](./README_KOR.md) | [Français](./README_FR.md) | [Português](./README_PTBR.md) | [Türkçe](./README_TR.md) | [Русский](./README_RU.md) | [Español](./README_ES.md) | [Italiano](./README_IT.md) | [ไทย](./README_TH.md) | [Deutsch](./README_DE.md) | [Tiếng Việt](./README_VI.md) | [עִברִית](https://github.com/elizaos/Elisa/blob/main/README_HE.md)

## ✨ Fonctionnalités

- 🛠️ Connecteurs complets pour Discord, Twitter et Telegram
- 🔗 Support pour chaque modèle (Llama, Grok, OpenAI, Anthropic, etc.)
- 👥 Support multi-agent et multi-salle
- 📚 Ingestion et interaction faciles avec vos documents
- 💾 Mémoire récupérable et stockage de documents
- 🚀 Hautement extensible - créez vos propres actions et clients
- ☁️ Supporte de nombreux modèles (Llama local, OpenAI, Anthropic, Groq, etc.)
- 📦 Ça fonctionne tout simplement !

## Tutoriels Vidéo

[AI Agent Dev School](https://www.youtube.com/watch?v=ArptLpQiKfI&list=PLx5pnFXdPTRzWla0RaOxALTSTnVq53fKL)

## 🎯 Cas d'utilisation

- 🤖 Chatbots
- 🕵️ Agents autonomes
- 📈 Gestion des processus d'affaires
- 🎮 PNJ de jeux vidéo
- 🧠 Trading

## 🚀 Démarrage rapide

### Prérequis

- [Python 2.7+](https://www.python.org/downloads/)
- [Node.js 23+](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- [pnpm](https://pnpm.io/installation)

> **Note pour les utilisateurs Windows :** [WSL 2](https://learn.microsoft.com/en-us/windows/wsl/install-manual) est requis.

### Utiliser le Starter (Recommandé)

```bash
git clone https://github.com/elizaos/eliza-starter.git
cd eliza-starter
cp .env.example .env
pnpm i && pnpm build && pnpm start
```

Ensuite, lisez la [Documentation](https://elizaos.github.io/eliza/) pour apprendre à personnaliser votre Eliza.

### Démarrer Eliza manuellement (Recommandé uniquement si vous savez ce que vous faites)

```bash
# Cloner le dépôt
git clone https://github.com/elizaos/eliza.git

# Passer à la dernière version
# Ce projet évolue rapidement, nous recommandons de passer à la dernière version
git checkout $(git describe --tags --abbrev=0)
```

### Démarrer Eliza avec Gitpod

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/elizaos/eliza/tree/main)

### Modifier le fichier .env

Copiez .env.example en .env et remplissez les valeurs appropriées.

```
cp .env.example .env
```

Note : .env est optionnel. Si vous prévoyez de faire fonctionner plusieurs agents distincts, vous pouvez passer les secrets via le JSON du personnage.

### Démarrage automatique d'Eliza

Cela exécutera tout pour configurer le projet et démarrer le bot avec le personnage par défaut.

```bash
sh scripts/start.sh
```

### Modifier le fichier de personnage

1. Ouvrez `packages/core/src/defaultCharacter.ts` pour modifier le personnage par défaut. Décommentez et modifiez.

2. Pour charger des personnages personnalisés :
    - Utilisez `pnpm start --characters="path/to/your/character.json"`
    - Plusieurs fichiers de personnages peuvent être chargés simultanément
3. Connectez-vous avec X (Twitter)
    - changez `"clients": []` en `"clients": ["twitter"]` dans le fichier de personnage pour vous connecter avec X

### Démarrer Eliza manuellement

```bash
pnpm i
pnpm build
pnpm start

# Le projet évolue rapidement, parfois vous devez nettoyer le projet si vous y revenez
pnpm clean
```

#### Exigences supplémentaires

Vous devrez peut-être installer Sharp. Si vous voyez une erreur au démarrage, essayez de l'installer avec la commande suivante :

```
pnpm install --include=optional sharp
```

### Communauté & contact

- [Problèmes GitHub](https://github.com/elizaos/eliza/issues). Idéal pour : les bugs que vous rencontrez en utilisant Eliza, et les propositions de fonctionnalités.
- [Discord](https://discord.gg/ai16z). Idéal pour : partager vos applications et discuter avec la communauté.

## Contributeurs

<a href="https://github.com/elizaos/eliza/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=elizaos/eliza" />
</a>

## Historique des étoiles

[![Star History Chart](https://api.star-history.com/svg?repos=elizaos/eliza&type=Date)](https://star-history.com/#elizaos/eliza&Date)