# Study Quiz App

A clean, fast quiz app for studying 500 multiple-choice questions across 10 modules.

## Features
- 10 modules of 50 questions each
- Shuffle mode per module
- Answer feedback with correct answer shown
- Progress tracking (saved in browser)
- Works on mobile and desktop

---

## How to Add Your Questions

Open `questions.js` and replace the placeholder questions with your real ones.

Each question follows this format:
```js
{
  id: 1,           // unique number (1–500)
  module: 1,       // which module (1–10)
  question: "What does DNS stand for?",
  options: [
    "Domain Name System",
    "Dynamic Network Service",
    "Data Node Subnet",
    "Distributed Name Server",
  ],
  correct: 0,      // index of the correct answer (0 = first option)
}
```

### Tips
- You can have 2, 3, or 4 options per question
- `correct` is zero-based: 0 = A, 1 = B, 2 = C, 3 = D
- Keep IDs unique across all 500 questions
- Module numbers 1–10, with 50 questions each

---

## Deploy to Vercel

1. Push this folder to a GitHub repository
2. Go to [vercel.com](https://vercel.com) and click **Add New → Project**
3. Import your GitHub repo
4. Framework Preset: **Other**
5. Click **Deploy** — done!

No build step needed. Vercel serves the static files directly.
