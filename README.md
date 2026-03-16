# 📄 WorksheetAI

> An AI-powered worksheet generator for teachers — enter any topic and get a fully formatted, print-ready worksheet with an answer key in seconds.

![HTML](https://img.shields.io/badge/HTML-Single%20File-orange?style=flat-square&logo=html5)
![Claude API](https://img.shields.io/badge/Claude-API-blueviolet?style=flat-square)
![License](https://img.shields.io/badge/License-Free%20for%20Education-green?style=flat-square)
![No Dependencies](https://img.shields.io/badge/Dependencies-None-lightgrey?style=flat-square)

---

## ✨ Features

- 🧠 **AI-generated questions** — Multiple Choice, Short Answer, True/False, Fill in the Blank, or Mixed
- 🎯 **Difficulty levels** — Easy, Medium, and Hard
- 🏫 **Grade levels** — Grade 4–5 up to College/University
- 🔑 **Answer Key** — full answers with explanations, toggle on/off
- 🖨️ **Print / PDF ready** — clean print layout at the click of a button
- ⚡ **No install needed** — everything runs in a single HTML file

---

## 🚀 Live Demo

> 🔗 **[your-username.github.io/your-repo-name](https://your-username.github.io/your-repo-name)**

*(Replace with your actual GitHub Pages URL after deploying)*

---

## 🛠️ Setup

### Step 1 — Get an Anthropic API Key

1. Go to [console.anthropic.com](https://console.anthropic.com) and sign up
2. Navigate to **API Keys** → create a new key
3. Copy the key — it starts with `sk-ant-...`

### Step 2 — Add Your API Key

Open `index.html` in a text editor. Find this section and paste your key:

```js
headers: {
  'Content-Type': 'application/json',
  'x-api-key': 'YOUR_API_KEY_HERE',
  'anthropic-version': '2023-06-01',
  'anthropic-dangerous-direct-browser-access': 'true'
},
```

> ⚠️ **Never commit your API key to a public repository.** See the [Security](#-security) section below.

### Step 3 — Deploy to GitHub Pages

1. Rename `worksheet-generator.html` to `index.html`
2. Push it to your repository
3. Go to your repo → **Settings** → **Pages**
4. Under **Source**, select `main` branch → `/ (root)`
5. Click **Save** — your site will be live in a few minutes at:

```
https://your-username.github.io/your-repo-name
```

---

## 📖 How to Use

| Step | Action |
|------|--------|
| 1 | Enter a **topic** — e.g. *Photosynthesis*, *World War II*, *Fractions* |
| 2 | Select the **grade level** |
| 3 | Pick a **difficulty** — Easy, Medium, or Hard |
| 4 | Choose a **question type** — Mixed or a specific format |
| 5 | Set the **number of questions** (3–20) |
| 6 | Add any **special instructions** (optional) |
| 7 | Click **Generate Worksheet** |
| 8 | Click **Show Answer Key** to reveal answers + explanations |
| 9 | Click **Print / Save PDF** for a clean printable version |

---

## 🔐 Security

This app calls the Anthropic API directly from the browser, which means the API key is visible in the source code.

| Use Case | Recommendation |
|----------|----------------|
| Personal / classroom use | ✅ Safe to use as-is |
| Shared with a small team | ✅ Password-protect the site (Netlify supports this) |
| Public website | ⚠️ Move the API call to a backend to hide your key |

**To keep your key private on GitHub**, never paste your real key into the HTML file before pushing. Instead, use a backend service (Node.js, Python, etc.) that holds the key server-side.

---

## 🗂️ File Structure

```
📦 your-repo-name
 ┣ 📄 index.html      # The entire application
 ┗ 📄 README.md       # This file
```

---

## 🧰 Tech Stack

| | Technology |
|---|---|
| Frontend | Vanilla HTML, CSS, JavaScript |
| AI Model | Anthropic Claude (`claude-sonnet-4-20250514`) |
| Fonts | Google Fonts — Crimson Pro + DM Sans |
| Dependencies | None |

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the repository
2. Create a new branch: `git checkout -b feature/my-feature`
3. Commit your changes: `git commit -m 'Add my feature'`
4. Push to the branch: `git push origin feature/my-feature`
5. Open a Pull Request

---

## 📄 License

Free to use for educational purposes. Not for resale or commercial distribution.

---

<p align="center">Made for teachers ✏️</p>
