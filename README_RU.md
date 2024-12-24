# Eliza 🤖

<div align="center">
  <img src="./docs/static/img/eliza_banner.jpg" alt="Eliza Banner" width="100%" />
</div>

<div align="center">

📖 [Документация](https://elizaos.github.io/eliza/) | 🎯 [Примеры](https://github.com/thejoven/awesome-eliza)

</div>

## 🌍 Переводы README

[中文说明](./README_CN.md) | [日本語の説明](./README_JA.md) | [한국어 설명](./README_KOR.md) | [Français](./README_FR.md) | [Português](./README_PTBR.md) | [Türkçe](./README_TR.md) | [Русский](./README_RU.md) | [Español](./README_ES.md) | [Italiano](./README_IT.md) | [ไทย](./README_TH.md) | [Deutsch](./README_DE.md) | [Tiếng Việt](./README_VI.md) | [עִברִית](https://github.com/elizaos/Elisa/blob/main/README_HE.md)

## ✨ Особенности

- 🛠️ Полнофункциональные коннекторы для Discord, Twitter и Telegram
- 🔗 Поддержка всех моделей (Llama, Grok, OpenAI, Anthropic и др.)
- 👥 Поддержка нескольких агентов и комнат
- 📚 Легкое взаимодействие с вашими документами
- 💾 Восстанавливаемая память и хранилище документов
- 🚀 Высокая расширяемость - создавайте свои собственные действия и клиенты
- ☁️ Поддержка множества моделей (локальная Llama, OpenAI, Anthropic, Groq и др.)
- 📦 Просто работает!

## Видеоуроки

[AI Agent Dev School](https://www.youtube.com/watch?v=ArptLpQiKfI&list=PLx5pnFXdPTRzWla0RaOxALTSTnVq53fKL)

## 🎯 Примеры использования

- 🤖 Чат-боты
- 🕵️ Автономные агенты
- 📈 Управление бизнес-процессами
- 🎮 NPC в видеоиграх
- 🧠 Трейдинг

## 🚀 Быстрый старт

### Предварительные требования

- [Python 2.7+](https://www.python.org/downloads/)
- [Node.js 23+](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- [pnpm](https://pnpm.io/installation)

> **Примечание для пользователей Windows:** требуется [WSL 2](https://learn.microsoft.com/en-us/windows/wsl/install-manual).

### Используйте Starter (рекомендуется)

```bash
git clone https://github.com/elizaos/eliza-starter.git
cd eliza-starter
cp .env.example .env
pnpm i && pnpm build && pnpm start
```

Затем прочитайте [Документацию](https://elizaos.github.io/eliza/), чтобы узнать, как настроить вашу Eliza.

### Запуск Eliza вручную (рекомендуется только если вы знаете, что делаете)

```bash
# Клонируйте репозиторий
git clone https://github.com/elizaos/eliza.git

# Переключитесь на последний релиз
# Этот проект быстро развивается, поэтому мы рекомендуем переключиться на последний релиз
git checkout $(git describe --tags --abbrev=0)
```

### Запуск Eliza с Gitpod

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/elizaos/eliza/tree/main)

### Редактирование файла .env

Скопируйте .env.example в .env и заполните соответствующими значениями.

```
cp .env.example .env
```

Примечание: .env не обязателен. Если вы планируете запускать несколько различных агентов, вы можете передавать секреты через JSON персонажа.

### Автоматический запуск Eliza

Это запустит все для настройки проекта и запуска бота с персонажем по умолчанию.

```bash
sh scripts/start.sh
```

### Редактирование файла персонажа

1. Откройте `packages/core/src/defaultCharacter.ts`, чтобы изменить персонажа по умолчанию. Раскомментируйте и отредактируйте.

2. Чтобы загрузить пользовательских персонажей:
    - Используйте `pnpm start --characters="path/to/your/character.json"`
    - Несколько файлов персонажей могут быть загружены одновременно
3. Подключение к X (Twitter)
    - измените `"clients": []` на `"clients": ["twitter"]` в файле персонажа для подключения к X

### Запуск Eliza вручную

```bash
pnpm i
pnpm build
pnpm start

# Проект быстро развивается, иногда вам нужно очистить проект, если вы возвращаетесь к нему
pnpm clean
```

#### Дополнительные требования

Возможно, вам потребуется установить Sharp. Если вы видите ошибку при запуске, попробуйте установить его с помощью следующей команды:

```
pnpm install --include=optional sharp
```

### Сообщество и контакты

- [GitHub Issues](https://github.com/elizaos/eliza/issues). Лучше всего для: ошибок, с которыми вы сталкиваетесь при использовании Eliza, и предложений по функциям.
- [Discord](https://discord.gg/ai16z). Лучше всего для: обмена вашими приложениями и общения с сообществом.

## Участники

<a href="https://github.com/elizaos/eliza/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=elizaos/eliza" />
</a>

## История звёзд

[![Star History Chart](https://api.star-history.com/svg?repos=elizaos/eliza&type=Date)](https://star-history.com/#elizaos/eliza&Date)