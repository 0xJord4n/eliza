# Eliza 🤖

<div align="center">
  <img src="./docs/static/img/eliza_banner.jpg" alt="Eliza Banner" width="100%" />
</div>

<div align="center">

📖 [Dokümantasyon](https://elizaos.github.io/eliza/) | 🎯 [Örnekler](https://github.com/thejoven/awesome-eliza)

</div>

## 🌍 README Çevirileri

[中文说明](./README_CN.md) | [日本語の説明](./README_JA.md) | [한국어 설명](./README_KOR.md) | [Français](./README_FR.md) | [Português](./README_PTBR.md) | [Türkçe](./README_TR.md) | [Русский](./README_RU.md) | [Español](./README_ES.md) | [Italiano](./README_IT.md) | [ไทย](./README_TH.md) | [Deutsch](./README_DE.md) | [Tiếng Việt](./README_VI.md) | [עִברִית](https://github.com/elizaos/Elisa/blob/main/README_HE.md)

## ✨ Özellikler

- 🛠️ Tam özellikli Discord, Twitter ve Telegram bağlayıcıları
- 🔗 Her model için destek (Llama, Grok, OpenAI, Anthropic, vb.)
- 👥 Çoklu ajan ve oda desteği
- 📚 Belgelerinizi kolayca içe aktarın ve etkileşimde bulunun
- 💾 Geri alınabilir hafıza ve belge deposu
- 🚀 Yüksek derecede genişletilebilir - kendi eylemlerinizi ve istemcilerinizi oluşturun
- ☁️ Birçok modeli destekler (yerel Llama, OpenAI, Anthropic, Groq, vb.)
- 📦 Sadece çalışır!

## Video Eğitimleri

[AI Ajan Geliştirme Okulu](https://www.youtube.com/watch?v=ArptLpQiKfI&list=PLx5pnFXdPTRzWla0RaOxALTSTnVq53fKL)

## 🎯 Kullanım Alanları

- 🤖 Sohbet botları
- 🕵️ Otonom Ajanlar
- 📈 İş Süreci Yönetimi
- 🎮 Video Oyun NPC'leri
- 🧠 Ticaret

## 🚀 Hızlı Başlangıç

### Gereksinimler

- [Python 2.7+](https://www.python.org/downloads/)
- [Node.js 23+](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- [pnpm](https://pnpm.io/installation)

> **Windows Kullanıcıları için Not:** [WSL 2](https://learn.microsoft.com/en-us/windows/wsl/install-manual) gereklidir.

### Başlangıç Kitini Kullanın (Önerilir)

```bash
git clone https://github.com/elizaos/eliza-starter.git
cd eliza-starter
cp .env.example .env
pnpm i && pnpm build && pnpm start
```

Daha sonra Eliza'nızı nasıl özelleştireceğinizi öğrenmek için [Dokümantasyonu](https://elizaos.github.io/eliza/) okuyun.

### Eliza'yı Manuel Başlatın (Sadece ne yaptığınızı biliyorsanız önerilir)

```bash
# Depoyu klonlayın
git clone https://github.com/elizaos/eliza.git

# En son sürüme geçin
# Bu proje hızlı bir şekilde iterasyon yapar, bu yüzden en son sürüme geçmenizi öneririz
git checkout $(git describe --tags --abbrev=0)
```

### Gitpod ile Eliza'yı Başlatın

[![Gitpod'da Aç](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/elizaos/eliza/tree/main)

### .env Dosyasını Düzenleyin

.env.example dosyasını .env olarak kopyalayın ve uygun değerleri doldurun.

```
cp .env.example .env
```

Not: .env isteğe bağlıdır. Birden fazla farklı ajan çalıştırmayı planlıyorsanız, karakter JSON üzerinden gizli bilgileri geçebilirsiniz.

### Eliza'yı Otomatik Başlatın

Bu, projeyi kurmak ve botu varsayılan karakterle başlatmak için her şeyi çalıştıracaktır.

```bash
sh scripts/start.sh
```

### Karakter Dosyasını Düzenleyin

1. Varsayılan karakteri değiştirmek için `packages/core/src/defaultCharacter.ts` dosyasını açın. Yorumları kaldırın ve düzenleyin.

2. Özel karakterleri yüklemek için:
    - `pnpm start --characters="path/to/your/character.json"` komutunu kullanın
    - Birden fazla karakter dosyası aynı anda yüklenebilir
3. X (Twitter) ile bağlanın
    - karakter dosyasında `"clients": []` ifadesini `"clients": ["twitter"]` olarak değiştirin

### Eliza'yı Manuel Başlatın

```bash
pnpm i
pnpm build
pnpm start

# Proje hızlı bir şekilde iterasyon yapar, projeye geri döndüğünüzde bazen projeyi temizlemeniz gerekebilir
pnpm clean
```

#### Ek Gereksinimler

Sharp'ı yüklemeniz gerekebilir. Başlangıçta bir hata görürseniz, aşağıdaki komutla yüklemeyi deneyin:

```
pnpm install --include=optional sharp
```

### Topluluk ve İletişim

- [GitHub Sorunları](https://github.com/elizaos/eliza/issues). En iyi kullanım alanı: Eliza'yı kullanırken karşılaştığınız hatalar ve özellik önerileri.
- [Discord](https://discord.gg/ai16z). En iyi kullanım alanı: uygulamalarınızı paylaşmak ve toplulukla vakit geçirmek.

## Katkıda Bulunanlar

<a href="https://github.com/elizaos/eliza/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=elizaos/eliza" />
</a>

## Yıldız Geçmişi

[![Yıldız Geçmişi Grafiği](https://api.star-history.com/svg?repos=elizaos/eliza&type=Date)](https://star-history.com/#elizaos/eliza&Date)