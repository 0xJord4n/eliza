# Eliza 🤖

<div align="center">
  <img src="./docs/static/img/eliza_banner.jpg" alt="Eliza Banner" width="100%" />
</div>

<div align="center">

📖 [ドキュメント](https://elizaos.github.io/eliza/) | 🎯 [例](https://github.com/thejoven/awesome-eliza)

</div>

## 🌍 READMEの翻訳

[中文说明](./README_CN.md) | [日本語の説明](./README_JA.md) | [한국어 설명](./README_KOR.md) | [Français](./README_FR.md) | [Português](./README_PTBR.md) | [Türkçe](./README_TR.md) | [Русский](./README_RU.md) | [Español](./README_ES.md) | [Italiano](./README_IT.md) | [ไทย](./README_TH.md) | [Deutsch](./README_DE.md) | [Tiếng Việt](./README_VI.md) | [עִברִית](https://github.com/elizaos/Elisa/blob/main/README_HE.md)

## ✨ 特徴

- 🛠️ フル機能のDiscord、Twitter、Telegramコネクタ
- 🔗 すべてのモデル（Llama、Grok、OpenAI、Anthropicなど）に対応
- 👥 マルチエージェントとルームサポート
- 📚 ドキュメントを簡単に取り込み、対話可能
- 💾 取得可能なメモリとドキュメントストア
- 🚀 高度に拡張可能 - 独自のアクションとクライアントを作成
- ☁️ 多くのモデルをサポート（ローカルLlama、OpenAI、Anthropic、Groqなど）
- 📦 すぐに使える！

## ビデオチュートリアル

[AIエージェント開発学校](https://www.youtube.com/watch?v=ArptLpQiKfI&list=PLx5pnFXdPTRzWla0RaOxALTSTnVq53fKL)

## 🎯 使用例

- 🤖 チャットボット
- 🕵️ 自律エージェント
- 📈 ビジネスプロセスの処理
- 🎮 ビデオゲームのNPC
- 🧠 トレーディング

## 🚀 クイックスタート

### 前提条件

- [Python 2.7+](https://www.python.org/downloads/)
- [Node.js 23+](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- [pnpm](https://pnpm.io/installation)

> **Windowsユーザーへの注意:** [WSL 2](https://learn.microsoft.com/en-us/windows/wsl/install-manual)が必要です。

### スターターを使用する（推奨）

```bash
git clone https://github.com/elizaos/eliza-starter.git
cd eliza-starter
cp .env.example .env
pnpm i && pnpm build && pnpm start
```

その後、[ドキュメント](https://elizaos.github.io/eliza/)を読んでElizaをカスタマイズする方法を学びましょう。

### Elizaを手動で開始する（知識がある場合のみ推奨）

```bash
# リポジトリをクローン
git clone https://github.com/elizaos/eliza.git

# 最新のリリースをチェックアウト
# このプロジェクトは迅速に進化するため、最新のリリースをチェックアウトすることをお勧めします
git checkout $(git describe --tags --abbrev=0)
```

### GitpodでElizaを開始

[![Gitpodで開く](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/elizaos/eliza/tree/main)

### .envファイルを編集

.env.exampleを.envにコピーし、適切な値を入力します。

```
cp .env.example .env
```

注意: .envはオプションです。複数の異なるエージェントを実行する予定がある場合、キャラクターJSONを通じてシークレットを渡すことができます。

### Elizaを自動的に開始

これにより、プロジェクトをセットアップし、デフォルトのキャラクターでボットを開始するためのすべてが実行されます。

```bash
sh scripts/start.sh
```

### キャラクターファイルを編集

1. `packages/core/src/defaultCharacter.ts`を開いてデフォルトのキャラクターを変更します。コメントを外して編集します。

2. カスタムキャラクターをロードするには:
    - `pnpm start --characters="path/to/your/character.json"`を使用
    - 複数のキャラクターファイルを同時にロード可能
3. X（Twitter）と接続するには
    - キャラクターファイルで`"clients": []`を`"clients": ["twitter"]`に変更

### Elizaを手動で開始

```bash
pnpm i
pnpm build
pnpm start

# プロジェクトは迅速に進化するため、プロジェクトに戻る際にはプロジェクトをクリーンにする必要がある場合があります
pnpm clean
```

#### 追加の要件

Sharpをインストールする必要があるかもしれません。起動時にエラーが表示された場合、次のコマンドでインストールを試みてください:

```
pnpm install --include=optional sharp
```

### コミュニティと連絡先

- [GitHub Issues](https://github.com/elizaos/eliza/issues). 最適: Elizaを使用中に遭遇したバグや機能提案。
- [Discord](https://discord.gg/ai16z). 最適: アプリケーションの共有やコミュニティとの交流。

## 貢献者

<a href="https://github.com/elizaos/eliza/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=elizaos/eliza" />
</a>

## スター履歴

[![スター履歴チャート](https://api.star-history.com/svg?repos=elizaos/eliza&type=Date)](https://star-history.com/#elizaos/eliza&Date)