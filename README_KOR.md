# 엘리자 🤖

<div align="center">
  <img src="./docs/static/img/eliza_banner.jpg" alt="Eliza Banner" width="100%" />
</div>

<div align="center">

📖 [문서](https://elizaos.github.io/eliza/) | 🎯 [예제](https://github.com/thejoven/awesome-eliza)

</div>

## 🌍 README 번역

[中文说明](./README_CN.md) | [日本語の説明](./README_JA.md) | [한국어 설명](./README_KOR.md) | [Français](./README_FR.md) | [Português](./README_PTBR.md) | [Türkçe](./README_TR.md) | [Русский](./README_RU.md) | [Español](./README_ES.md) | [Italiano](./README_IT.md) | [ไทย](./README_TH.md) | [Deutsch](./README_DE.md) | [Tiếng Việt](./README_VI.md) | [עִברִית](https://github.com/elizaos/Elisa/blob/main/README_HE.md)

## ✨ 기능

- 🛠️ 디스코드, 트위터, 텔레그램의 완전한 기능의 커넥터
- 🔗 모든 모델 지원 (Llama, Grok, OpenAI, Anthropic 등)
- 👥 다중 에이전트 및 룸 지원
- 📚 문서를 쉽게 수집하고 상호작용
- 💾 검색 가능한 메모리 및 문서 저장소
- 🚀 매우 확장 가능 - 자신만의 액션과 클라이언트 생성
- ☁️ 다양한 모델 지원 (로컬 Llama, OpenAI, Anthropic, Groq 등)
- 📦 바로 작동!

## 비디오 튜토리얼

[AI 에이전트 개발 학교](https://www.youtube.com/watch?v=ArptLpQiKfI&list=PLx5pnFXdPTRzWla0RaOxALTSTnVq53fKL)

## 🎯 사용 사례

- 🤖 챗봇
- 🕵️ 자율 에이전트
- 📈 비즈니스 프로세스 처리
- 🎮 비디오 게임 NPC
- 🧠 트레이딩

## 🚀 빠른 시작

### 사전 준비

- [Python 2.7+](https://www.python.org/downloads/)
- [Node.js 23+](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- [pnpm](https://pnpm.io/installation)

> **Windows 사용자 참고:** [WSL 2](https://learn.microsoft.com/en-us/windows/wsl/install-manual)가 필요합니다.

### 스타터 사용 (권장)

```bash
git clone https://github.com/elizaos/eliza-starter.git
cd eliza-starter
cp .env.example .env
pnpm i && pnpm build && pnpm start
```

그런 다음 [문서](https://elizaos.github.io/eliza/)를 읽고 엘리자를 사용자 정의하는 방법을 배우세요.

### 엘리자 수동 시작 (권장하지 않음)

```bash
# 리포지토리 클론
git clone https://github.com/elizaos/eliza.git

# 최신 릴리스 체크아웃
# 이 프로젝트는 빠르게 반복되므로 최신 릴리스를 체크아웃하는 것이 좋습니다.
git checkout $(git describe --tags --abbrev=0)
```

### Gitpod로 엘리자 시작

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/elizaos/eliza/tree/main)

### .env 파일 편집

.env.example을 .env로 복사하고 적절한 값을 입력하세요.

```
cp .env.example .env
```

참고: .env는 선택 사항입니다. 여러 개의 개별 에이전트를 실행하려는 경우, 캐릭터 JSON을 통해 비밀을 전달할 수 있습니다.

### 엘리자 자동 시작

이 명령은 프로젝트를 설정하고 기본 캐릭터로 봇을 시작하는 모든 작업을 수행합니다.

```bash
sh scripts/start.sh
```

### 캐릭터 파일 편집

1. `packages/core/src/defaultCharacter.ts`를 열어 기본 캐릭터를 수정합니다. 주석을 해제하고 편집하세요.

2. 사용자 정의 캐릭터를 로드하려면:
    - `pnpm start --characters="path/to/your/character.json"`을 사용하세요.
    - 여러 캐릭터 파일을 동시에 로드할 수 있습니다.
3. X (트위터)와 연결:
    - 캐릭터 파일에서 `"clients": []`를 `"clients": ["twitter"]`로 변경하여 X와 연결하세요.

### 엘리자 수동 시작

```bash
pnpm i
pnpm build
pnpm start

# 프로젝트가 빠르게 반복되므로, 프로젝트로 돌아올 때 프로젝트를 정리해야 할 수도 있습니다.
pnpm clean
```

#### 추가 요구 사항

시작 시 오류가 발생하면 Sharp를 설치해야 할 수 있습니다. 다음 명령으로 설치해보세요:

```
pnpm install --include=optional sharp
```

### 커뮤니티 & 연락처

- [GitHub 이슈](https://github.com/elizaos/eliza/issues). 엘리자를 사용하면서 발생하는 버그 및 기능 제안에 가장 적합합니다.
- [디스코드](https://discord.gg/ai16z). 애플리케이션을 공유하고 커뮤니티와 함께하는 데 가장 적합합니다.

## 기여자

<a href="https://github.com/elizaos/eliza/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=elizaos/eliza" />
</a>

## 스타 히스토리

[![Star History Chart](https://api.star-history.com/svg?repos=elizaos/eliza&type=Date)](https://star-history.com/#elizaos/eliza&Date)