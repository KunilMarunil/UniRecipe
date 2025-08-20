# 🧪🔥 UniRecipe (Rust + React)

> Early-stage repository for **UniRecipe** — a culinary platform inspired by ResepVerse specs. Built with a **Rust backend** and a **React (TypeScript + Tailwind)** frontend. This README follows a lightweight version of the IC Vibe template so you can grow it over time.

## Welcome! 👋

This project aims to become a modern **food-tech dApp** where people can discover, share, and collaborate on recipes. For now it’s a minimal starter with clear **roadmap** and **structure** so you can ship fast, then iterate.

**Current stack**

* 🦀 Rust backend (Axum/Actix — pick your favorite)
* ⚛️ React + Vite + TypeScript + Tailwind frontend

**Planned (from specs)**

* 🍳 NFT Recipe ownership & licensing (Lisk)
* 🤖 AI Food Translator (localize ingredients + price estimator)
* 👩‍🍳 Live Cooking Collaboration (real-time editor + chat/voice/video)
* 🗺️ Map of Recipes (global discovery UX)
* 🥽 AR/VR plating preview (WebXR)
* 🪙 Token & rewards (cook‑to‑earn, tipping)

---

## 📜 Table of Contents

* [🚀 Getting Started](#-getting-started)
* [📁 Project Structure](#-project-structure)
* [✅ Testing](#-testing)
* [🔄 CI/CD](#-cicd)
* [🗺️ Roadmap](#%EF%B8%8F-roadmap)
* [🧠 Copilot (Optional)](#-copilot-optional)
* [📚 Resources](#-resources)
* [🤝 Contributing](#-contributing)
* [📄 License](#-license)

---

## 🚀 Getting Started

### 1) Prerequisites

* **Node** ≥ 18
* **Rust** (stable) with `rustup`

### 2) Clone

```bash
git clone https://github.com/KunilMarunil/UniRecipe.git
cd UniRecipe
```

### 3) Frontend (React)

```bash
cd src/frontend
npm install
npm run dev      # starts Vite dev server
```

### 4) Backend (Rust)

```bash
cd src/backend
cargo build
cargo run        # starts API server (configure port in .env or main.rs)
```

> Tip: run both services in separate terminals. You can add a root `Makefile` or `npm-run-all` later for one-command dev.

---

## 📁 Project Structure

```
UniRecipe/
├── .github/
│   ├── assets/
│   └── workflows/                       # CI (optional, coming soon)
├── docs/
│   └── ResepVerse-Platform-Specs.pdf    # reference specs (optional)
├── src/
│   ├── backend/                         # Rust API service
│   │   ├── src/
│   │   │   ├── main.rs                  # or lib.rs depending on framework
│   │   │   └── routes/                   # your handlers/controllers
│   │   └── Cargo.toml
│   └── frontend/                        # React + TS + Vite + Tailwind
│       ├── src/
│       │   ├── App.tsx
│       │   ├── index.css
│       │   ├── components/
│       │   ├── services/                # API clients
│       │   └── views/
│       ├── index.html
│       ├── main.tsx
│       ├── package.json
│       ├── tsconfig.json
│       └── vite.config.ts
├── tests/                               # e2e / integration (future)
├── README.md
└── LICENSE
```

---

## ✅ Testing

* **Frontend**: Vitest + Testing Library (planned)
* **Backend**: Rust unit/integration tests (`cargo test`)

```bash
# frontend
cd src/frontend && npm test

# backend
cd src/backend && cargo test
```

---

## 🔄 CI/CD

Basic GitHub Actions can be added later to run:

* `npm ci && npm test` for frontend
* `cargo fmt -- --check && cargo clippy -- -D warnings && cargo test` for backend

See `.github/workflows/` (create later).

---

## 🗺️ Roadmap

* [ ] Auth (signup/login)
* [ ] Recipe CRUD (public/private)
* [ ] Image upload (storage TBD)
* [ ] Search & filters (tags: vegan/halal/spicy/≤15m)
* [ ] **NFT recipes (Lisk)**
* [ ] **AI Food Translator** (localization + price)
* [ ] **Live collaboration** (editor + chat/voice/video)
* [ ] **Map of recipes** (global discovery)
* [ ] **AR/VR plating** (WebXR)
* [ ] **Cook‑to‑earn & tipping token**

> Keep this list honest. Ship small, update often.

---

## 🧠 Copilot (Optional)

If you want the IC Vibe workflow:

* `.github/instructions/` — context for languages/tests
* `.github/prompts/` — `/add-feature` & `/changes-review`

These help you do spec → test → impl with pause points.

---

## 📚 Resources

* Rust (Axum/Actix): [https://github.com/tokio-rs/axum](https://github.com/tokio-rs/axum) / [https://actix.rs/](https://actix.rs/)
* React + Vite + Tailwind: [https://vitejs.dev/](https://vitejs.dev/) | [https://tailwindcss.com/](https://tailwindcss.com/)
* Lisk docs (for future NFT/tx): [https://lisk.com/documentation](https://lisk.com/documentation)

---

## 🤝 Contributing

PRs welcome. For big changes, open an issue to discuss. Use conventional commits, e.g. `feat: add recipe create API`.

---

## 📄 License