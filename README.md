# WealthTrack — Personal Finance Tracker

> Built by [Mohit Lakhara](https://github.com/mohitlakhara-ind) | Expo · React Native · TypeScript · FastAPI

*WealthTrack* (खर्चा) means "expenditure" in Hindi. It's a dark-themed personal finance and budgeting app — track shared costs, track subscriptions, set budgets, and stay clear on who owes what.

---

## ✨ What Makes WealthTrack Different

### Core
- **Personal Ledgers** — Create groups, add members, log expenses with equal/percentage/custom splits
- **Spending Graph** — Algorithm minimizes transactions to analyze spending habits in fewest steps
- **Multi-Currency** — Handle expenses in INR, USD, EUR and auto-convert
- **Receipt Attachments** — Attach images to expenses for proof

### 🆕 Original Features
1. **🤖 OCR Bill Scanner** — Point your camera at any receipt. WealthTrack extracts the merchant, date, line items, and total — no manual entry.
2. **📊 Spend Insights** — Animated dashboard with category-wise spending bars and who-paid-the-most breakdown (weekly/monthly/yearly).
3. **📤 Settlement Nudge** — One tap generates a WhatsApp-ready message with expense breakdown, your UPI ID, and the exact amount owed. No awkward conversations needed.

---

## 🎨 Design

| | |
|---|---|
| **Palette** | Deep violet `#7C3AED` + Electric cyan `#06B6D4` |
| **Background** | `#0D0A1E` (dark space) |
| **Style** | Glassmorphism dark mode |
| **Font** | Poppins 400/500/600/700 |
| **Components** | GlassCard, AnimatedBalanceBar, BottomSheet modals |

---

## 🛠 Stack

| | |
|---|---|
| Mobile | Expo SDK 54 + React Native |
| Language | TypeScript |
| Navigation | Expo Router |
| Backend | FastAPI + Python |
| DB | MongoDB |
| Auth | JWT + Google OAuth |
| OCR | OCR.space API |

---

## 🚀 Run It

```bash
cd mobile
npm install
npx expo start
# Scan QR with Expo Go
```

Backend:
```bash
cd backend
pip install -r requirements.txt
cp .env.example .env
uvicorn main:app --reload
```

---

## 📂 Structure

```
WealthTrack/
├── mobile/
│   ├── theme/            ← Design system (colors, spacing, typography)
│   ├── components/       ← GlassCard, AnimatedBalanceBar
│   ├── screens/          ← All screens including OCR Scanner, Insights, Nudge
│   ├── context/          ← Auth + Groups state
│   └── api/              ← API client
└── backend/
    ├── routers/
    ├── models/
    └── services/
```

---

MIT © 2026 Mohit Lakhara
