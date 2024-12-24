# Eliza 🤖

<div align="center">
  <img src="./docs/static/img/eliza_banner.jpg" alt="Eliza Banner" width="100%" />
</div>

<div align="center">

📖 [เอกสาร](https://elizaos.github.io/eliza/) | 🎯 [ตัวอย่าง](https://github.com/thejoven/awesome-eliza)

</div>

## 🌍 README แปลภาษา

[中文说明](./README_CN.md) | [日本語の説明](./README_JA.md) | [한국어 설명](./README_KOR.md) | [Français](./README_FR.md) | [Português](./README_PTBR.md) | [Türkçe](./README_TR.md) | [Русский](./README_RU.md) | [Español](./README_ES.md) | [Italiano](./README_IT.md) | [ไทย](./README_TH.md) | [Deutsch](./README_DE.md) | [Tiếng Việt](./README_VI.md) | [עִברִית](https://github.com/elizaos/Elisa/blob/main/README_HE.md)

## ✨ คุณสมบัติ

- 🛠️ ตัวเชื่อมต่อ Discord, Twitter และ Telegram ที่มีคุณสมบัติครบถ้วน
- 🔗 รองรับทุกโมเดล (Llama, Grok, OpenAI, Anthropic, ฯลฯ)
- 👥 รองรับหลายเอเจนต์และห้อง
- 📚 สามารถนำเข้าและโต้ตอบกับเอกสารของคุณได้อย่างง่ายดาย
- 💾 หน่วยความจำและที่เก็บเอกสารที่สามารถเรียกคืนได้
- 🚀 ขยายได้สูง - สร้างการกระทำและลูกค้าของคุณเอง
- ☁️ รองรับหลายโมเดล (Llama ในเครื่อง, OpenAI, Anthropic, Groq, ฯลฯ)
- 📦 ใช้งานได้ทันที!

## วิดีโอสอน

[AI Agent Dev School](https://www.youtube.com/watch?v=ArptLpQiKfI&list=PLx5pnFXdPTRzWla0RaOxALTSTnVq53fKL)

## 🎯 กรณีการใช้งาน

- 🤖 แชทบอท
- 🕵️ เอเจนต์อัตโนมัติ
- 📈 การจัดการกระบวนการธุรกิจ
- 🎮 NPC ในวิดีโอเกม
- 🧠 การซื้อขาย

## 🚀 เริ่มต้นอย่างรวดเร็ว

### ข้อกำหนดเบื้องต้น

- [Python 2.7+](https://www.python.org/downloads/)
- [Node.js 23+](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- [pnpm](https://pnpm.io/installation)

> **หมายเหตุสำหรับผู้ใช้ Windows:** [WSL 2](https://learn.microsoft.com/en-us/windows/wsl/install-manual) จำเป็นต้องใช้

### ใช้ Starter (แนะนำ)

```bash
git clone https://github.com/elizaos/eliza-starter.git
cd eliza-starter
cp .env.example .env
pnpm i && pnpm build && pnpm start
```

จากนั้นอ่าน [เอกสาร](https://elizaos.github.io/eliza/) เพื่อเรียนรู้วิธีปรับแต่ง Eliza ของคุณ

### เริ่ม Eliza ด้วยตนเอง (แนะนำเฉพาะถ้าคุณรู้ว่ากำลังทำอะไรอยู่)

```bash
# โคลนที่เก็บ
git clone https://github.com/elizaos/eliza.git

# ตรวจสอบรุ่นล่าสุด
# โครงการนี้พัฒนาอย่างรวดเร็ว ดังนั้นเราขอแนะนำให้ตรวจสอบรุ่นล่าสุด
git checkout $(git describe --tags --abbrev=0)
```

### เริ่ม Eliza ด้วย Gitpod

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/elizaos/eliza/tree/main)

### แก้ไขไฟล์ .env

คัดลอก .env.example ไปยัง .env และกรอกค่าที่เหมาะสม

```
cp .env.example .env
```

หมายเหตุ: .env เป็นทางเลือก หากคุณวางแผนที่จะเรียกใช้เอเจนต์ที่แตกต่างกันหลายตัว คุณสามารถส่งความลับผ่าน JSON ของตัวละคร

### เริ่ม Eliza โดยอัตโนมัติ

สิ่งนี้จะเรียกใช้ทุกอย่างเพื่อตั้งค่าโครงการและเริ่มบอทด้วยตัวละครเริ่มต้น

```bash
sh scripts/start.sh
```

### แก้ไขไฟล์ตัวละคร

1. เปิด `packages/core/src/defaultCharacter.ts` เพื่อแก้ไขตัวละครเริ่มต้น ยกเลิกการคอมเมนต์และแก้ไข

2. เพื่อโหลดตัวละครที่กำหนดเอง:
    - ใช้ `pnpm start --characters="path/to/your/character.json"`
    - สามารถโหลดไฟล์ตัวละครหลายไฟล์พร้อมกันได้
3. เชื่อมต่อกับ X (Twitter)
    - เปลี่ยน `"clients": []` เป็น `"clients": ["twitter"]` ในไฟล์ตัวละครเพื่อเชื่อมต่อกับ X

### เริ่ม Eliza ด้วยตนเอง

```bash
pnpm i
pnpm build
pnpm start

# โครงการนี้พัฒนาอย่างรวดเร็ว บางครั้งคุณจำเป็นต้องล้างโครงการหากคุณกลับมาที่โครงการ
pnpm clean
```

#### ข้อกำหนดเพิ่มเติม

คุณอาจจำเป็นต้องติดตั้ง Sharp หากคุณเห็นข้อผิดพลาดเมื่อเริ่มต้น ลองติดตั้งด้วยคำสั่งต่อไปนี้:

```
pnpm install --include=optional sharp
```

### ชุมชน & ติดต่อ

- [ปัญหาใน GitHub](https://github.com/elizaos/eliza/issues). เหมาะสำหรับ: ข้อบกพร่องที่คุณพบเมื่อใช้ Eliza และข้อเสนอแนะคุณสมบัติ
- [Discord](https://discord.gg/ai16z). เหมาะสำหรับ: แบ่งปันแอปพลิเคชันของคุณและพูดคุยกับชุมชน

## ผู้ร่วมพัฒนา

<a href="https://github.com/elizaos/eliza/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=elizaos/eliza" />
</a>

## ประวัติดาว

[![Star History Chart](https://api.star-history.com/svg?repos=elizaos/eliza&type=Date)](https://star-history.com/#elizaos/eliza&Date)