# אליזה 🤖

<div align="center">
  <img src="./docs/static/img/eliza_banner.jpg" alt="אליזה באנר" width="100%" />
</div>

<div align="center">

📖 [תיעוד](https://elizaos.github.io/eliza/) | 🎯 [דוגמאות](https://github.com/thejoven/awesome-eliza)

</div>

## 🌍 תרגומי README

[中文说明](./README_CN.md) | [日本語の説明](./README_JA.md) | [한국어 설명](./README_KOR.md) | [Français](./README_FR.md) | [Português](./README_PTBR.md) | [Türkçe](./README_TR.md) | [Русский](./README_RU.md) | [Español](./README_ES.md) | [Italiano](./README_IT.md) | [ไทย](./README_TH.md) | [Deutsch](./README_DE.md) | [Tiếng Việt](./README_VI.md) | [עִברִית](https://github.com/elizaos/Elisa/blob/main/README_HE.md)

## ✨ תכונות

- 🛠️ מחברים מלאים לדיסקורד, טוויטר וטלגרם
- 🔗 תמיכה בכל מודל (Llama, Grok, OpenAI, Anthropic, וכו')
- 👥 תמיכה בריבוי סוכנים וחדרים
- 📚 קל לבלוע ולתקשר עם המסמכים שלך
- 💾 זיכרון ומאגר מסמכים ניתנים לשליפה
- 🚀 ניתן להרחבה גבוהה - צור פעולות ולקוחות משלך
- ☁️ תומך בהרבה מודלים (Llama מקומי, OpenAI, Anthropic, Groq, וכו')
- 📦 פשוט עובד!

## מדריכי וידאו

[AI Agent Dev School](https://www.youtube.com/watch?v=ArptLpQiKfI&list=PLx5pnFXdPTRzWla0RaOxALTSTnVq53fKL)

## 🎯 מקרי שימוש

- 🤖 צ'אטבוטים
- 🕵️ סוכנים אוטונומיים
- 📈 ניהול תהליכים עסקיים
- 🎮 NPCs במשחקי וידאו
- 🧠 מסחר

## 🚀 התחלה מהירה

### דרישות מוקדמות

- [Python 2.7+](https://www.python.org/downloads/)
- [Node.js 23+](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
- [pnpm](https://pnpm.io/installation)

> **הערה למשתמשי Windows:** [WSL 2](https://learn.microsoft.com/en-us/windows/wsl/install-manual) נדרש.

### השתמש ב-Starter (מומלץ)

```bash
git clone https://github.com/elizaos/eliza-starter.git
cd eliza-starter
cp .env.example .env
pnpm i && pnpm build && pnpm start
```

לאחר מכן קרא את [התיעוד](https://elizaos.github.io/eliza/) כדי ללמוד כיצד להתאים אישית את אליזה שלך.

### הפעל את אליזה ידנית (מומלץ רק אם אתה יודע מה אתה עושה)

```bash
# שיבוט המאגר
git clone https://github.com/elizaos/eliza.git

# מעבר לגרסה האחרונה
# הפרויקט מתעדכן במהירות, לכן אנו ממליצים לעבור לגרסה האחרונה
git checkout $(git describe --tags --abbrev=0)
```

### הפעל את אליזה עם Gitpod

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/elizaos/eliza/tree/main)

### ערוך את קובץ ה-.env

העתק את .env.example ל-.env ומלא את הערכים המתאימים.

```
cp .env.example .env
```

הערה: .env הוא אופציונלי. אם אתה מתכנן להפעיל מספר סוכנים נפרדים, תוכל להעביר סודות דרך ה-JSON של הדמות

### הפעל את אליזה אוטומטית

זה יריץ הכל כדי להגדיר את הפרויקט ולהפעיל את הבוט עם הדמות המוגדרת כברירת מחדל.

```bash
sh scripts/start.sh
```

### ערוך את קובץ הדמות

1. פתח `packages/core/src/defaultCharacter.ts` כדי לשנות את הדמות המוגדרת כברירת מחדל. בטל הערה וערוך.

2. כדי לטעון דמויות מותאמות אישית:
    - השתמש ב-`pnpm start --characters="path/to/your/character.json"`
    - ניתן לטעון מספר קבצי דמויות בו זמנית
3. התחבר עם X (טוויטר)
    - שנה `"clients": []` ל-`"clients": ["twitter"]` בקובץ הדמות כדי להתחבר עם X

### הפעל את אליזה ידנית

```bash
pnpm i
pnpm build
pnpm start

# הפרויקט מתעדכן במהירות, לפעמים תצטרך לנקות את הפרויקט אם אתה חוזר אליו
pnpm clean
```

#### דרישות נוספות

ייתכן שתצטרך להתקין את Sharp. אם אתה רואה שגיאה בעת ההפעלה, נסה להתקין אותו עם הפקודה הבאה:

```
pnpm install --include=optional sharp
```

### קהילה ויצירת קשר

- [בעיות GitHub](https://github.com/elizaos/eliza/issues). הכי טוב עבור: באגים שאתה נתקל בהם בשימוש באליזה, והצעות לפיצ'רים.
- [Discord](https://discord.gg/ai16z). הכי טוב עבור: שיתוף היישומים שלך והתחברות עם הקהילה.

## תורמים

<a href="https://github.com/elizaos/eliza/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=elizaos/eliza" />
</a>

## היסטוריית כוכבים

[![Star History Chart](https://api.star-history.com/svg?repos=elizaos/eliza&type=Date)](https://star-history.com/#elizaos/eliza&Date)