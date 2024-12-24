# Eliza 🤖

<div align="center">
  <img src="./docs/static/img/eliza_banner.jpg" alt="Eliza Banner" width="100%" />
</div>

<div align="center">

📖 [Tài liệu](https://elizaos.github.io/eliza/) | 🎯 [Ví dụ](https://github.com/thejoven/awesome-eliza)

</div>

## 🌍 Bản dịch README

[中文说明](./README_CN.md) | [日本語の説明](./README_JA.md) | [한국어 설명](./README_KOR.md) | [Français](./README_FR.md) | [Português](./README_PTBR.md) | [Türkçe](./README_TR.md) | [Русский](./README_RU.md) | [Español](./README_ES.md) | [Italiano](./README_IT.md) | [ไทย](./README_TH.md) | [Deutsch](./README_DE.md) | [Tiếng Việt](./README_VI.md) | [עִברִית](https://github.com/elizaos/Elisa/blob/main/README_HE.md)

## ✨ Tính năng

- 🛠️ Kết nối đầy đủ với Discord, Twitter và Telegram
- 🔗 Hỗ trợ cho mọi mô hình (Llama, Grok, OpenAI, Anthropic, v.v.)
- 👥 Hỗ trợ đa tác nhân và phòng
- 📚 Dễ dàng nhập và tương tác với tài liệu của bạn
- 💾 Bộ nhớ và kho tài liệu có thể truy xuất
- 🚀 Rất dễ mở rộng - tạo hành động và khách hàng của riêng bạn
- ☁️ Hỗ trợ nhiều mô hình (Llama cục bộ, OpenAI, Anthropic, Groq, v.v.)
- 📦 Chỉ cần hoạt động!

## Video Hướng dẫn

[Trường Phát triển Tác nhân AI](https://www.youtube.com/watch?v=ArptLpQiKfI&list=PLx5pnFXdPTRzWla0RaOxALTSTnVq53fKL)

## 🎯 Trường hợp sử dụng

- 🤖 Chatbots
- 🕵️ Tác nhân tự động
- 📈 Xử lý quy trình kinh doanh
- 🎮 NPC trong trò chơi điện tử
- 🧠 Giao dịch

## 🚀 Bắt đầu nhanh

### Yêu cầu

- [Python 2.7+](https://www.python.org/downloads/)
- [Node.js 23+](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- [pnpm](https://pnpm.io/installation)

> **Lưu ý cho người dùng Windows:** [WSL 2](https://learn.microsoft.com/en-us/windows/wsl/install-manual) là cần thiết.

### Sử dụng Starter (Khuyến nghị)

```bash
git clone https://github.com/elizaos/eliza-starter.git
cd eliza-starter
cp .env.example .env
pnpm i && pnpm build && pnpm start
```

Sau đó đọc [Tài liệu](https://elizaos.github.io/eliza/) để tìm hiểu cách tùy chỉnh Eliza của bạn.

### Khởi động Eliza thủ công (Chỉ khuyến nghị nếu bạn biết mình đang làm gì)

```bash
# Clone kho lưu trữ
git clone https://github.com/elizaos/eliza.git

# Chuyển sang phiên bản phát hành mới nhất
# Dự án này phát triển nhanh, vì vậy chúng tôi khuyến nghị chuyển sang phiên bản phát hành mới nhất
git checkout $(git describe --tags --abbrev=0)
```

### Khởi động Eliza với Gitpod

[![Mở trong Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/elizaos/eliza/tree/main)

### Chỉnh sửa tệp .env

Sao chép .env.example thành .env và điền các giá trị phù hợp.

```
cp .env.example .env
```

Lưu ý: .env là tùy chọn. Nếu bạn dự định chạy nhiều tác nhân khác nhau, bạn có thể truyền các bí mật thông qua JSON của nhân vật

### Tự động khởi động Eliza

Điều này sẽ chạy mọi thứ để thiết lập dự án và khởi động bot với nhân vật mặc định.

```bash
sh scripts/start.sh
```

### Chỉnh sửa tệp nhân vật

1. Mở `packages/core/src/defaultCharacter.ts` để chỉnh sửa nhân vật mặc định. Bỏ chú thích và chỉnh sửa.

2. Để tải các nhân vật tùy chỉnh:
    - Sử dụng `pnpm start --characters="path/to/your/character.json"`
    - Nhiều tệp nhân vật có thể được tải đồng thời
3. Kết nối với X (Twitter)
    - thay đổi `"clients": []` thành `"clients": ["twitter"]` trong tệp nhân vật để kết nối với X

### Khởi động Eliza thủ công

```bash
pnpm i
pnpm build
pnpm start

# Dự án phát triển nhanh, đôi khi bạn cần làm sạch dự án nếu bạn quay lại dự án
pnpm clean
```

#### Yêu cầu bổ sung

Bạn có thể cần cài đặt Sharp. Nếu bạn thấy lỗi khi khởi động, hãy thử cài đặt nó với lệnh sau:

```
pnpm install --include=optional sharp
```

### Cộng đồng & liên hệ

- [Vấn đề trên GitHub](https://github.com/elizaos/eliza/issues). Tốt nhất cho: lỗi bạn gặp phải khi sử dụng Eliza và đề xuất tính năng.
- [Discord](https://discord.gg/ai16z). Tốt nhất cho: chia sẻ ứng dụng của bạn và giao lưu với cộng đồng.

## Người đóng góp

<a href="https://github.com/elizaos/eliza/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=elizaos/eliza" />
</a>

## Lịch sử sao

[![Biểu đồ Lịch sử Sao](https://api.star-history.com/svg?repos=elizaos/eliza&type=Date)](https://star-history.com/#elizaos/eliza&Date)