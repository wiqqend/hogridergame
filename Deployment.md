# 🚀 Deployment Guide for Type-to-Move Platformer

This document explains how to deploy and run your **Type-to-Move Platformer** game locally or online.

---

## 🧩 Project Overview

This game is a **browser-based platformer** built with HTML, CSS, and JavaScript. It features type-to-move mechanics, background music, jump and death sound effects, and a start menu.

---

## 🖥️ Local Deployment (Play on Your Computer)

### Step 1: Download or Copy Project Files

Ensure your project folder contains:
```
index.html
jump.mp3
dead.mp3
music.mp3
```

> You can include other assets such as images, level files, or additional sound effects.

### Step 2: Run Locally

To test locally, open `index.html` in your browser.

#### Option A – Double-click:
Simply **double-click** the `index.html` file.

#### Option B – Local server (recommended):
If you encounter audio or script issues due to browser security restrictions, serve the game locally:

**Using VS Code (Recommended):**
1. Install the **Live Server** extension.
2. Right-click `index.html` → **Open with Live Server**.

**Using Command Line:**
```bash
# Python 3.x
python -m http.server 8000
```
Then open: [http://localhost:8000](http://localhost:8000)

---

## 🌍 Online Deployment (Play on the Web)

### Option 1: GitHub Pages (Free)

1. Go to your GitHub account.
2. Create a new repository — name it something like `type-to-move-platformer`.
3. Upload all files (`index.html`, `music.mp3`, `jump.mp3`, `dead.mp3`, etc.).
4. Go to **Settings → Pages**.
5. Under “Build and deployment,” set:
   - **Source:** Deploy from branch
   - **Branch:** `main` (or `master`)
6. Click **Save**.

GitHub will provide a URL like:
```
https://yourusername.github.io/type-to-move-platformer/
```
Your game will be live there! 🎮

---

### Option 2: Itch.io (for Indie Game Hosting)

1. Go to [https://itch.io](https://itch.io) and create an account.
2. Click **Upload new project**.
3. Set **Kind of project** → `HTML (playable in browser)`.
4. Upload your zipped folder (containing index.html and assets).
5. Check **"This file will be played in the browser"**.
6. Publish — your game is instantly available online.

---

### Option 3: Netlify (Advanced & Custom Domain Support)

1. Go to [https://netlify.com](https://netlify.com).
2. Sign up and click **Add new site → Deploy manually**.
3. Drag and drop your project folder.
4. Done — your game will get a live `.netlify.app` URL!

---

## 🧱 Folder Structure Example

```
/type-to-move-platformer
│
├── index.html
├── jump.mp3
├── dead.mp3
├── music.mp3
└── Deployment.md
```

---

## 🔊 Audio Tips

- Keep file names lowercase with no spaces.
- Use `.mp3` or `.ogg` for maximum browser support.
- Adjust volumes in JavaScript if needed:
```js
jumpSound.volume = 0.7;
deadSound.volume = 1.0; // Louder death sound
music.volume = 0.5;
```

---

## ⚙️ Troubleshooting

| Issue | Cause | Fix |
|-------|--------|-----|
| Audio doesn’t play | Browser blocks autoplay | Start music after user input (e.g. clicking Start button) |
| Controls not responding | Wrong file paths or console errors | Open DevTools (F12) → Console tab |
| Game not loading online | Missing files or case-sensitive file names | Ensure all asset names match exactly |

---

## 🏁 That’s It!

Your **Type-to-Move Platformer** is ready to play and share.  
Happy coding and gaming! 🎮🔥
