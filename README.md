# 🧠 PolymarketWatcher Bot

**PolymarketWatcher** is a real-time monitoring bot that automatically detects and posts **new [Polymarket](https://polymarket.com)** markets and **whale trades** to a Telegram channel.  
Built in **Python**, designed for stability, automation, and 24/7 operation.

![Python](https://img.shields.io/badge/python-3.10%2B-blue)
![Polymarket API](https://img.shields.io/badge/Polymarket-API-orange)
![Telegram Bot](https://img.shields.io/badge/Telegram-Bot-blue)

---

## 🚀 Features

- 🔍 **Real-time market tracking** via the [Polymarket Gamma API](https://docs.polymarket.com/developers/CLOB/endpoints)  
- 🕒 Filters markets by creation or update date (`createdAt` / `updatedAt`)  
- 💾 Prevents duplicate posts via `posted_markets.json`  
- 🐋 Whale detection for trades above **$5,000 USD**  
- 💬 Telegram integration for clean, HTML-formatted messages  
- 🛠 Runs under **systemd** on Ubuntu (auto restart & logging)  
- 📊 All events are logged to `bot_log.txt`  

---

## ⚙️ How It Works

1. Fetches market data from **Polymarket Gamma API**  
2. Filters new or updated markets (only after Oct 28, 2025)  
3. Posts new markets to Telegram  
4. Optionally scans whale trades  
5. Saves posted markets locally to prevent duplicates  

---

## 🧩 Tech Stack

| Component | Description |
|------------|--------------|
| **Language** | Python 3 |
| **Libraries** | requests, json, datetime |
| **API** | Polymarket Gamma API |
| **Runtime** | Ubuntu 24.04 / WSL2 |
| **Integration** | Telegram Bot API |

---

## 🧠 Benefits

- Fully automated, runs 24/7  
- Instant Telegram alerts for new markets  
- Lightweight and low resource usage  
- Transparent logs for easy debugging  
- Perfect for analysts and crypto traders  

---

## 📦 Installation Guide

```bash
# 1. Clone repository
git clone https://github.com/timurg405/polymarket-watcher-bot.git
cd polymarket-watcher-bot

# 2. Create and activate virtual environment
python3 -m venv venv
source venv/bin/activate

# 3. Install dependencies
pip install requests

# 4. Run the bot manually
python3 bot.py



🔗 Live Updates

📢 Follow live market updates here:
👉 t.me/PolymarketWatcher

💬 Credits

Built with ❤️ by @timurg405

Inspired by the amazing prediction market platform @Polymarket
