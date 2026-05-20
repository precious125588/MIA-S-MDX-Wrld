# 🜲  MIAS MDX  ·  MIA'S MDX ·  v4.9.9

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=28&duration=2600&pause=600&color=8AE234&center=true&vCenter=true&multiline=true&width=820&height=110&lines=%E2%9A%A1+MIAS+MDX+%E2%80%94+WhatsApp+Super-Bot;%F0%9F%A7%A0+powered+by+NIX+Assistant+v1.0;%F0%9F%94%92+Encrypted+%C2%B7+Obfuscated+%C2%B7+Battle-tested" alt="MIAS MDX" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/node-%3E%3D18-43A047?style=for-the-badge&logo=node.js&logoColor=white" />
  <img src="https://img.shields.io/badge/baileys-1.0.4--rc.5-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" />
  <img src="https://img.shields.io/badge/build-obfuscated-8E24AA?style=for-the-badge&logo=lock&logoColor=white" />
  <img src="https://img.shields.io/badge/status-online-00C853?style=for-the-badge" />
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24&height=140&section=header&reversal=true" width="100%"/>
</p>

---

## ⚡  GRAB YOUR SESSION ID

> The bot needs a **SESSION_ID** to log in. Generate one here:

<p align="center">
  <a href="https://season-mias-test-production-4404.up.railway.app/">
    <img src="https://img.shields.io/badge/🜲%20PAIR%20YOUR%20SESSION-Open%20Generator-25D366?style=for-the-badge&logoColor=white" />
  </a>
</p>

```
https://season-mias-test-production-4404.up.railway.app/
```

Paste the generated string into `.env` as `SESSION_ID=...` and you're live.

<p align="center">
  <img src="https://user-images.githubusercontent.com/74038190/212284100-561aa473-3905-4a80-b561-0d28506553ee.gif" width="100%"/>
</p>

---

## 🧠  WHAT THIS BOT CAN DO

### 👤  Account Intelligence
`contacts` · `unread` · `blocked` · `archived` · `report` · `status` · `clearstatus`

### 💬  Messaging & Contacts
`text` · `block` · `unblock` · `add` · `forward` · `delete`

### 👥  Group Management
`groups` · `groupstats` · `members` · `activegroups` · `inactivegroups`
`kick` · `kickadmins` · `close` · `open` · `mute` · `unmute`
`promote` · `promoteall` · `demote` · `demoteall`
`tagall` · `invite` · `revoke` · `leave` · `gcban` · `groupsummary`

### 🤖  AI Assistant (NIX core)
`ai` · `summarize` · `rewrite` · `translate` · `explain`
`poem` · `story` · `code` · `fix` · `roast` · `define` · `synonym`

### 🎧  Media Tools
`download` · `sticker` · `gif` · `meme` · `video` · `moviedl` (doc-mode)
`viewonce` · `saveviewonce` · `lastmedia` · `mediafrom` · `mediasent`
M4A MIME fix · PDF → text · sticker-first reactions

### 🕵️  Contact Intelligence
`profile` · `about` · `lastseen` · `online` · `contactinfo`
`lastmsg` · `firstmsg` · `msgcount` · `searchmsg`
`deleted` · `edited` · `mostactive` · `leastactive`
`chatreport` · `streak` · `lastcall` · `missedcalls` · `lastdoc` · `finddoc`

### ⚙️  System Tools
`uptime` · `ping` · `health` · `logs` · `version` · `stats` · `reset`

### 🌐  Info & Web
`weather` · `news` · `wiki` · `search` · `fact` · `joke` · `quote`
`calculate` · `myip`

### 📝  Productivity
`note` · `notes` · `todo` · `todos` · `remind`

### 🛒  Panel Selling
Built-in panel store · custom price · contact · description from `.env`

### 🗣️  Natural Language Mode
Just talk to it. No prefix required:
```
"Nix kick this person"
"Nix download this video"
"Nix summarize this chat"
"Nix text 2349012345678 hello"
"Nix what's the weather in Lagos"
```

### 📡  Owner Tools
`broadcast` (DM-only) · auto owner-detection · multi-owner · `setnixowner`

<p align="center">
  <img src="https://user-images.githubusercontent.com/74038190/216122041-518ac897-8d92-4c6b-9b3f-ca01dcaf38ee.png" width="60"/>
  <img src="https://user-images.githubusercontent.com/74038190/216122003-1de8d44d-e1da-4e80-9c89-22cce58d4c52.png" width="60"/>
  <img src="https://user-images.githubusercontent.com/74038190/216122069-5b8169d7-1d8e-4a13-b245-a8e4176c99f8.png" width="60"/>
</p>

---


## 🚀  DEPLOY

```bash
# 1. install
npm install

# 2. configure
cp .env.example .env
nano .env          # paste SESSION_ID + OWNER_NAME

# 3. fly
npm start
```

### Host anywhere
- **Render** — `Procfile` included
- **Railway** — auto-detects `npm start`
- **Heroku** — works out of the box
- **Pterodactyl / VPS** — `node --expose-gc --max-old-space-size=896 index.js`

---

## 📁  STRUCTURE

```
mias_mdx/
├── index.js              ← entry (obfuscated · light profile)
├── api.js                ← APIs (obfuscated · heavy)
├── database.js           ← persistence (obfuscated · heavy)
├── davidcyril.js         ← scraper bridge (obfuscated · heavy)
├── nix/                  ← NIX assistant core (all obfuscated · heavy)
│   ├── index.js  intent.js  menu.js  ui.js  owner.js  api.js
│   └── modules/          ← 10 capability modules
├── assets/               ← bot pic, menu cover, sfx (untouched)
├── .env.example          ← template
├── owner.json            ← runtime state
├── Procfile · package.json
```

---

## 🧾  ENV TEMPLATE

```env
SESSION_ID=prezzy_PASTE_FROM_LINK_ABOVE
OWNER_NAME=𝑷𝑹𝑬𝑪𝑰𝑶𝑼𝑺 x
BOT_NAME=MIAS MDX
PREFIX=.
PANEL_URL=
PANEL_PRICE=DM for pricing
NIX_OWNER_NAME=𝑷𝑹𝑬𝑪𝑰𝑶𝑼𝑺 x
HF_TOKEN=
OPENAI_API_KEY=
```

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,24&height=120&section=footer" width="100%"/>
</p>

<p align="center">
  <b>MIAS MDX v4.9.9 · obfuscated build</b><br/>
  <sub>made loud · run silent</sub>
</p>
