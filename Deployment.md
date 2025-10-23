# 🕹️ Type-to-Move Platformer
### Deployment & Usage Guide

**Developed by:** Jacob & Jamie  
**Project Type:** HTML5 / JavaScript Web Game  
**Version:** 1.0  
**Date:** October 2025  

---

## 📁 1. Project Overview

**Type-to-Move Platformer** is a retro-styled, command-based platformer game where the player controls a character by typing commands such as `jump`, `left`, or `right`.  
The project is built entirely in **HTML, CSS, and JavaScript**, requiring no external dependencies or installation of libraries.

Players can explore randomly generated terrain, collect coins, avoid enemies, and survive dangerous lava pits — all while listening to dynamic sound effects and background music.

---

## ⚙️ 2. System Requirements

**Minimum Requirements:**
- Modern Web Browser (Google Chrome, Microsoft Edge, Firefox, or Safari)
- JavaScript enabled
- Audio support for MP3 files
- Screen resolution of **at least 1200×600 pixels**

**Recommended:**
- Desktop or laptop computer (the game is not optimized for mobile)
- Chrome Browser for best performance and audio playback

---

## 📂 3. Project Structure
Your project folder should contain the following files:

/TypeToMovePlatformer

│

├── index.html # Main HTML file (the game)

├── hoggif.png # Player sprite (Hog Rider)

├── goblin.png # Enemy sprite

├── head.png # Coin sprite

├── menu.png # Logo for start menu

│

├── menuaudio.mp3 # Background menu/game music

├── run.mp3 # Running sound effect

├── jump.mp3 # Jump sound effect

├── dead.mp3 # Death sound effect

│

└── (Optional) README.txt # Additional notes/documentation



---

## 🚀 4. Deployment Instructions

### Option 1 — Run Locally
1. Ensure all game files are in the same folder as shown above.
2. Open the folder on your computer.
3. **Double-click** the `index.html` file.  
   → This will open the game in your default web browser.
4. The game starts with the **Start Menu**.  
   Click the **Start** button to begin.

> 💡 If the background music does not start automatically, click anywhere inside the game window (browser audio restrictions may block autoplay).

---

### Option 2 — Host on a Web Server
You can deploy this project to any static web host, such as:
- GitHub Pages
- Netlify
- Vercel
- Replit
- Localhost via VS Code Live Server extension

**Steps for GitHub Pages:**
1. Create a new GitHub repository and upload all files.
2. Go to **Settings → Pages**.
3. Under *Build and Deployment*, select `Deploy from branch`.
4. Choose the `main` branch and `/ (root)` directory.
5. Wait for the deployment and open the provided URL.

---

## 🧭 5. Gameplay Instructions

### 🎮 Starting the Game
- Click **Start** on the title screen.
- Background music (`menuaudio.mp3`) begins.
- The player spawns on the left side of the screen.

### ✏️ Typing Commands
Use the **text box** below the game canvas to type commands.  
Press **Enter** after typing each command.

**Available Commands:**
| Command | Description |
|----------|--------------|
| `left` or `back` | Move left |
| `right` or `forward` | Move right |
| `jump` | Jump upward |
| `pause` | Pause the game |
| `unpause` | Resume the game |
| `menu` | Open the pause menu |
| `bio` | Show developer bios |
| `testmode` | Unlock arrow key controls for testing |

---

### ⌨️ Test Mode Controls
Once `testmode` is enabled, you can use:
- **ArrowRight** → Move right  
- **ArrowLeft** → Move left  
- **ArrowUp** → Jump  

This mode is primarily for debugging or casual play.

---

## 🔊 6. Audio Behavior

| Sound | File | Trigger |
|--------|------|----------|
| Background Music | `menuaudio.mp3` | Starts when game begins |
| Jump Sound | `jump.mp3` | Each jump command |
| Run Sound | `run.mp3` | Each movement command |
| Death Sound | `dead.mp3` | When the player dies |

> The **death sound** is intentionally set to *high volume* for dramatic effect.

---

## 💀 7. Death & Reset Logic
- The player dies if:
  - Falling into **lava**
  - Colliding with an **enemy**
  - Falling below the screen
- When the player dies:
  - The game pauses
  - `dead.mp3` plays
  - A Game Over alert shows the score
  - The player resets to the starting position

---

## 🧱 8. Game Features Summary

✅ Random terrain generation  
✅ Dynamic sky color fading  
✅ Collectible coins  
✅ Platform gaps and floating platforms  
✅ Real-time scoring system  
✅ Responsive sound effects  
✅ Developer bios popup  
✅ Command-based input system  
✅ Debug/Test mode with arrow key support  

---

## 🧩 9. Troubleshooting

| Issue | Cause | Fix |
|--------|--------|-----|
| **No sound** | Browser blocks autoplay | Click anywhere inside the page before starting |
| **Player doesn’t move** | Forgot to type “Enter” after a command | Always press Enter to execute |
| **Lava not showing** | Missing terrain generation | Refresh or check console for errors |
| **Sprites not visible** | Wrong file path or missing image | Ensure all `.png` files are in same folder |
| **Game doesn’t start** | Missing Start button click | Click **Start** in the start menu to begin |

---

## 🧑‍💻 10. Developer Notes

- The game logic, physics, and rendering loop are all written in **vanilla JavaScript** (no frameworks).
- The map is procedurally generated using random height shifts and lava gaps.
- All rendering is done via the **HTML5 Canvas API**.
- Fonts and graphics are styled for a retro arcade aesthetic using `Press Start 2P`.

---

## 📜 11. License & Credits

**Developers:**  
- Jamie — Visual design, menus, and bio system  
- Jacob — Core gameplay, command logic, and sound integration  

**Assets:**  
- Sprites & sound effects created by the developers or sourced from royalty-free libraries.  
- Font: *Press Start 2P* by Codeman38 (Google Fonts)

**License:** Educational / Non-commercial use permitted.
