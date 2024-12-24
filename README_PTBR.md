# Eliza 🤖

<div align="center">
  <img src="./docs/static/img/eliza_banner.jpg" alt="Eliza Banner" width="100%" />
</div>

<div align="center">

📖 [Documentação](https://elizaos.github.io/eliza/) | 🎯 [Exemplos](https://github.com/thejoven/awesome-eliza)

</div>

## 🌍 Traduções do README

[中文说明](./README_CN.md) | [日本語の説明](./README_JA.md) | [한국어 설명](./README_KOR.md) | [Français](./README_FR.md) | [Português](./README_PTBR.md) | [Türkçe](./README_TR.md) | [Русский](./README_RU.md) | [Español](./README_ES.md) | [Italiano](./README_IT.md) | [ไทย](./README_TH.md) | [Deutsch](./README_DE.md) | [Tiếng Việt](./README_VI.md) | [עִברִית](https://github.com/elizaos/Elisa/blob/main/README_HE.md)

## ✨ Funcionalidades

- 🛠️ Conectores completos para Discord, Twitter e Telegram
- 🔗 Suporte para todos os modelos (Llama, Grok, OpenAI, Anthropic, etc.)
- 👥 Suporte para múltiplos agentes e salas
- 📚 Ingestão e interação fácil com seus documentos
- 💾 Memória recuperável e armazenamento de documentos
- 🚀 Altamente extensível - crie suas próprias ações e clientes
- ☁️ Suporta muitos modelos (Llama local, OpenAI, Anthropic, Groq, etc.)
- 📦 Funciona perfeitamente!

## Tutoriais em Vídeo

[AI Agent Dev School](https://www.youtube.com/watch?v=ArptLpQiKfI&list=PLx5pnFXdPTRzWla0RaOxALTSTnVq53fKL)

## 🎯 Casos de Uso

- 🤖 Chatbots
- 🕵️ Agentes Autônomos
- 📈 Gestão de Processos de Negócio
- 🎮 NPCs em Jogos de Vídeo
- 🧠 Trading

## 🚀 Início Rápido

### Pré-requisitos

- [Python 2.7+](https://www.python.org/downloads/)
- [Node.js 23+](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- [pnpm](https://pnpm.io/installation)

> **Nota para Usuários do Windows:** [WSL 2](https://learn.microsoft.com/en-us/windows/wsl/install-manual) é necessário.

### Use o Starter (Recomendado)

```bash
git clone https://github.com/elizaos/eliza-starter.git
cd eliza-starter
cp .env.example .env
pnpm i && pnpm build && pnpm start
```

Depois leia a [Documentação](https://elizaos.github.io/eliza/) para aprender como personalizar seu Eliza.

### Inicie Eliza Manualmente (Recomendado apenas se você souber o que está fazendo)

```bash
# Clone o repositório
git clone https://github.com/elizaos/eliza.git

# Faça checkout da última versão
# Este projeto evolui rapidamente, então recomendamos fazer checkout da última versão
git checkout $(git describe --tags --abbrev=0)
```

### Inicie Eliza com Gitpod

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/elizaos/eliza/tree/main)

### Edite o arquivo .env

Copie .env.example para .env e preencha os valores apropriados.

```
cp .env.example .env
```

Nota: .env é opcional. Se você planeja executar múltiplos agentes distintos, pode passar segredos através do JSON do personagem.

### Inicie Eliza Automaticamente

Isso executará tudo para configurar o projeto e iniciar o bot com o personagem padrão.

```bash
sh scripts/start.sh
```

### Edite o arquivo de personagem

1. Abra `packages/core/src/defaultCharacter.ts` para modificar o personagem padrão. Descomente e edite.

2. Para carregar personagens personalizados:
    - Use `pnpm start --characters="path/to/your/character.json"`
    - Múltiplos arquivos de personagens podem ser carregados simultaneamente
3. Conecte-se com X (Twitter)
    - mude `"clients": []` para `"clients": ["twitter"]` no arquivo de personagem para conectar com X

### Inicie Eliza Manualmente

```bash
pnpm i
pnpm build
pnpm start

# O projeto evolui rapidamente, às vezes você precisa limpar o projeto se estiver voltando para ele
pnpm clean
```

#### Requisitos Adicionais

Você pode precisar instalar o Sharp. Se você ver um erro ao iniciar, tente instalá-lo com o seguinte comando:

```
pnpm install --include=optional sharp
```

### Comunidade & contato

- [GitHub Issues](https://github.com/elizaos/eliza/issues). Melhor para: bugs que você encontrar usando Eliza e propostas de funcionalidades.
- [Discord](https://discord.gg/ai16z). Melhor para: compartilhar suas aplicações e interagir com a comunidade.

## Contribuidores

<a href="https://github.com/elizaos/eliza/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=elizaos/eliza" />
</a>

## Histórico de Estrelas

[![Star History Chart](https://api.star-history.com/svg?repos=elizaos/eliza&type=Date)](https://star-history.com/#elizaos/eliza&Date)