# Eliza 🤖

<div align="center">
  <img src="./docs/static/img/eliza_banner.jpg" alt="Eliza Banner" width="100%" />
</div>

<div align="center">

📖 [Documentación](https://elizaos.github.io/eliza/) | 🎯 [Ejemplos](https://github.com/thejoven/awesome-eliza)

</div>

## 🌍 Traducciones del README

[中文说明](./README_CN.md) | [日本語の説明](./README_JA.md) | [한국어 설명](./README_KOR.md) | [Français](./README_FR.md) | [Português](./README_PTBR.md) | [Türkçe](./README_TR.md) | [Русский](./README_RU.md) | [Español](./README_ES.md) | [Italiano](./README_IT.md) | [ไทย](./README_TH.md) | [Deutsch](./README_DE.md) | [Tiếng Việt](./README_VI.md) | [עִברִית](https://github.com/elizaos/Elisa/blob/main/README_HE.md)

## ✨ Características

- 🛠️ Conectores completos para Discord, Twitter y Telegram
- 🔗 Soporte para cada modelo (Llama, Grok, OpenAI, Anthropic, etc.)
- 👥 Soporte multi-agente y de salas
- 📚 Ingesta e interacción fácil con tus documentos
- 💾 Memoria recuperable y almacenamiento de documentos
- 🚀 Altamente extensible - crea tus propias acciones y clientes
- ☁️ Soporta muchos modelos (Llama local, OpenAI, Anthropic, Groq, etc.)
- 📦 ¡Funciona sin más!

## Tutoriales en Video

[Escuela de Desarrollo de Agentes de IA](https://www.youtube.com/watch?v=ArptLpQiKfI&list=PLx5pnFXdPTRzWla0RaOxALTSTnVq53fKL)

## 🎯 Casos de Uso

- 🤖 Chatbots
- 🕵️ Agentes Autónomos
- 📈 Manejo de Procesos de Negocio
- 🎮 NPCs en Videojuegos
- 🧠 Trading

## 🚀 Inicio Rápido

### Prerrequisitos

- [Python 2.7+](https://www.python.org/downloads/)
- [Node.js 23+](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- [pnpm](https://pnpm.io/installation)

> **Nota para Usuarios de Windows:** Se requiere [WSL 2](https://learn.microsoft.com/en-us/windows/wsl/install-manual).

### Usa el Starter (Recomendado)

```bash
git clone https://github.com/elizaos/eliza-starter.git
cd eliza-starter
cp .env.example .env
pnpm i && pnpm build && pnpm start
```

Luego lee la [Documentación](https://elizaos.github.io/eliza/) para aprender cómo personalizar tu Eliza.

### Iniciar Eliza Manualmente (Solo recomendado si sabes lo que estás haciendo)

```bash
# Clona el repositorio
git clone https://github.com/elizaos/eliza.git

# Cambia a la última versión
# Este proyecto itera rápido, por lo que recomendamos cambiar a la última versión
git checkout $(git describe --tags --abbrev=0)
```

### Inicia Eliza con Gitpod

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/elizaos/eliza/tree/main)

### Edita el archivo .env

Copia .env.example a .env y completa los valores apropiados.

```
cp .env.example .env
```

Nota: .env es opcional. Si planeas ejecutar múltiples agentes distintos, puedes pasar secretos a través del JSON del personaje.

### Inicia Eliza Automáticamente

Esto ejecutará todo para configurar el proyecto e iniciar el bot con el personaje predeterminado.

```bash
sh scripts/start.sh
```

### Edita el archivo de personaje

1. Abre `packages/core/src/defaultCharacter.ts` para modificar el personaje predeterminado. Descomenta y edita.

2. Para cargar personajes personalizados:
    - Usa `pnpm start --characters="path/to/your/character.json"`
    - Se pueden cargar múltiples archivos de personajes simultáneamente
3. Conéctate con X (Twitter)
    - cambia `"clients": []` a `"clients": ["twitter"]` en el archivo de personaje para conectarte con X

### Inicia Eliza Manualmente

```bash
pnpm i
pnpm build
pnpm start

# El proyecto itera rápido, a veces necesitas limpiar el proyecto si estás regresando al proyecto
pnpm clean
```

#### Requisitos Adicionales

Puede que necesites instalar Sharp. Si ves un error al iniciar, intenta instalarlo con el siguiente comando:

```
pnpm install --include=optional sharp
```

### Comunidad y contacto

- [GitHub Issues](https://github.com/elizaos/eliza/issues). Mejor para: errores que encuentres usando Eliza y propuestas de características.
- [Discord](https://discord.gg/ai16z). Mejor para: compartir tus aplicaciones y pasar el rato con la comunidad.

## Contribuidores

<a href="https://github.com/elizaos/eliza/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=elizaos/eliza" />
</a>

## Historial de Estrellas

[![Star History Chart](https://api.star-history.com/svg?repos=elizaos/eliza&type=Date)](https://star-history.com/#elizaos/eliza&Date)