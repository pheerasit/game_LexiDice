# Tower of Language (LexiDice)

A dice-battle RPG for learning English vocabulary. Climb a 6-floor tower, fight a boss on each floor, and use your knowledge of English words, especially **antonyms**, to win.

**Play online:** https://game-lexidice-2.onrender.com/

---

## Story

The Tower of Language has imprisoned the language crystals. As the hero, you must climb all 6 floors, defeat each guardian, and reclaim the crystals.

## How to Play

### 1. Dice Battles
- Choose a difficulty from the main menu: 🌱 **Easy** · ⚔️ **Normal** · 💀 **Hard**. Beginners should start with Easy.
- Turns alternate between **Attack** ⚔️ and **Defense** 🛡️.
- Both sides roll dice. **Damage = attack roll − defense roll.**

### 2. Skill Cards & Language Runes
Press **Skill** and answer a language rune question. There are 4 question types:

| Rune | Task |
|---|---|
| 🔮 Antonym | Choose the opposite word |
| 📘 Meaning | Choose the Thai meaning |
| 📜 Scroll | Fill in the missing word in a sentence |
| 👂 Echo | Listen to the word and choose it |

- Skills cost ⚡ **energy** (max 10). You regain energy by hitting the boss, taking hits, blocking fully, and answering correctly.
- **Correct answer:** you get a power-up, such as ×2 attack, a weaker boss roll, a shield, or healing. You also earn a ⭐.
- **Wrong answer / time out:** the effect backfires on you.
- Answer within half the time limit to earn bonus 🪙 coins.

### 3. Ultimate & Weapons
- Collect **3 ⭐** to unlock **💥 Ultimate Roll** for massive damage.
- Choose a weapon at the start: **Sword**, **Magic Staff**, or **Bow**. Each has its own bonuses.

### 4. Lucky Money Mini-game & Shop
- After beating a boss, play a spelling mini-game to earn 🪙 gold.
- Visit the **Wandering Shop** to buy Max HP potions, armor, revival feathers, or a new weapon.

### 5. Training Hall
- Words you answer wrong are saved to your 📕 **Review List** automatically.
- Practice 10 untimed questions. Score 7 or more to earn a 💎 crystal, which turns into 🪙 coins on your next adventure.

## The 6 Floors

| Floor | Boss | Vocabulary Theme | Words |
|---|---|---|---|
| 1 | Mirror Wolf | Size & Quantity | 16 |
| 2 | Archive Keeper | Feelings | 16 |
| 3 | Chrono Golem | Time & Speed | 16 |
| 4 | Abyss Warden | Nature | 16 |
| 5 | Mirror General | Actions | 16 |
| 6 | The Inverted King | Qualities | 16 |

**96 words in total**, organized as antonym pairs (e.g. *Big ↔ Small*, *Happy ↔ Sad*, *Fast ↔ Slow*). Bosses on floors 2–6 each have a special spell with its own question style, such as listen-only or words spelled backwards.

## Features
- 🌐 Switch the interface between **Thai and English** (vocabulary stays bilingual)
- 🔊 Word pronunciation with the browser's text-to-speech
- 📖 **Codex** of all vocabulary and boss info
- 💾 **3 save slots**, plus save export/import as a file
- 🎵 Boss battle music and sound effects
- 📱 Works on desktop and mobile (landscape mode)

## Run Locally

The game is a single HTML file. You can open `index.html` in a browser directly, but music and images load more reliably from a local server:

```bash
npm install
npm start
```

Then open the URL shown in the terminal.

## Project Structure

```
index.html                    # The whole game (HTML, CSS, JavaScript)
package.json                  # Static server for deployment (serve)
boss_bgm.mp3                  # Boss battle music
ชั้น 1 Entrance Floor.jpeg   # Floor/boss images (floors 1–6)
...
ชั้น 6 Throne Floor.jpeg
```

## Deployment

Hosted on [Render](https://render.com) as a Web Service:
- **Build command:** `yarn`
- **Start command:** `yarn start` (runs `npx serve -s . -l $PORT`)

You can also deploy it as a **Static Site** with an empty build command and publish directory `.`.

## Tools Used

### AI Tools
- **[Claude](https://claude.ai)** (Anthropic): AI assistant for coding, debugging, and documentation
- **[Google Antigravity](https://antigravity.google)**: AI-powered IDE for development

### Development & Hosting
- **HTML, CSS, JavaScript**: the whole game runs in the browser with no framework
- **Web Audio API & Web Speech API**: sound effects and word pronunciation
- **[GitHub](https://github.com)**: source code hosting
- **[Render](https://render.com)**: deployment

## Credits
- Music: *Eldenia Music Pack* (Royalty Free RPG Music)
- Developed by **pheerasit**
