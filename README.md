<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=1,6,30&height=180&section=header&text=Rekt+Run&fontSize=56&fontColor=000000&fontAlignY=38&desc=Lane-runner+game+as+a+Farcaster+mini+app+%E2%80%94+survive+the+rekt+zone&descAlignY=58&descSize=14&animation=fadeIn" width="100%"/>

<div align="center">

[![Play](https://img.shields.io/badge/Play%20Now-bbf7d0?style=for-the-badge&logoColor=000)](https://rekt-run.vercel.app)
[![License](https://img.shields.io/badge/MIT-bfdbfe?style=for-the-badge&logoColor=000)](LICENSE)
[![Platform](https://img.shields.io/badge/Farcaster%20Mini%20App-fde68a?style=for-the-badge&logoColor=000)]()
[![Tech](https://img.shields.io/badge/JavaScript%20%2B%20Vite-fca5a5?style=for-the-badge&logoColor=000)]()

</div>

<div align="center">
<i>Dodge the rekt zone in a fast lane-runner game built as a Farcaster mini app .... save scores to a leaderboard and optionally commit them on-chain.</i>
</div>

---

## ✦ Features

<div align="center">

| | Feature | What it does |
|:---:|---|---|
| 🏃 | Lane-runner gameplay | Dodge obstacles across lanes, survive as long as possible |
| 🏆 | Local leaderboard | Stores top scores in localStorage by default |
| ⛓️ | On-chain score option | Can be extended with a backend for on-chain submissions |
| 📱 | Farcaster native | Runs inside Warpcast / Base app as a mini app |
| 💰 | Tip support | Built-in tip configuration for Base Mainnet |

</div>

---

## ✦ Download & Run

**Step 1** .... Clone the repo

```bash
git clone https://github.com/0xnurrabby/RektRun
cd RektRun
```

**Step 2** .... Install dependencies

```bash
npm install
```

**Step 3** .... Start dev server

```bash
npm run dev
# Open http://localhost:5173
```

---

## ✦ Setup

```
1. Clone the repo and run npm install
2. Run npm run dev and open http://localhost:5173
3. Before publishing as an official mini app, sign the manifest:
   Edit public/.well-known/farcaster.json and replace:
   - accountAssociation.header
   - accountAssociation.payload
   - accountAssociation.signature
   (generate these via Base Build Preview or Farcaster Manifest Tool)
4. In src/main.js set:
   - RECIPIENT to your checksummed EVM address
   - BUILDER_CODE to your program-issued builder code
5. Build for production: npm run build
6. Deploy the dist/ folder to Vercel
```

---

## ✦ Project Structure

```
RektRun/
  src/
    main.js        ->  game engine, lane logic, wallet, leaderboard
  public/
    .well-known/   ->  Farcaster app manifest
    assets/        ->  sprites, icons, embed images
  index.html       ->  entry point with Farcaster mini app meta
  package.json
  vite.config.js
  vercel.json
```

---

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=1,6,30&height=100&section=footer&animation=fadeIn" width="100%"/>

<div align="center">MIT License .... built by <a href="https://github.com/0xnurrabby">0xnurrabby</a></div>
