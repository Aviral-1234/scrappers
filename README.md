# 🏴‍☠️ The Scraping Hub

This repo is a graveyard for any and all scrapers I feel like writing.  
It’s modular, chaotic, and it gets the job done.

---

## 📂 Layout

Every scraper gets its own folder. If it’s here, it works (or it did when I wrote it).

```
/scrapers - The actual guts. Each sub-folder is a different target  
/shared - Boilerplate logic—user-agents, proxy rotators, and DB connectors  
/data - Where the loot goes (Git-ignored by default)
```

---

## 🛠 Setup

Don't overcomplicate it.

### 1. Clone the repo

```bash
git clone <repo_url>
```

### 2. Environment setup

Copy `.env.example` to `.env` and add your proxies / keys.

```bash
cp .env.example .env
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🚀 How to Use

Navigate to whatever scraper you want to run and fire it off.

```bash
python scrapers/whatever_site/main.py
```

---

## 📜 The Rules

### ❌ Don't Commit Data
Keep your massive JSON/CSV files out of commits.

### ❌ Don't Commit Keys
Put your API tokens and proxy credentials in `.env`.

### ⚠️ Don't Break the Site
Use the shared delays so you don't get IP banned in five minutes.

---

## 📊 Current Arsenal

| Module | Target | Tech | Status |
|------|------|------|------|
| `scrapers/example` | Some Site | Playwright | 🟢 Running |
| `scrapers/api_hit` | Some API | Requests | 🟡 Fragile |

---

## 🧠 Note

If a scraper breaks because the site changed its UI for the 5th time this week, that's life.  

Fix it or delete it.
