# Afyniti Bot Scripts 🚀

This collection of Python scripts automates task completion on the Afyniti platform — a Web3 quest ecosystem where users earn XP by completing social tasks, daily quizzes, attendance check-ins, and Twitter/X account linking.

🔗 Register: [Afyniti](https://afyniti.xyz?ref=IK87HXQS)

---

## ✨ Features Overview

### General Features

- **Multi-Account Support**: Reads private keys from `pvkey.txt` to process multiple accounts in parallel.
- **Central Menu System**: Interactive menu for easy script selection via `main.py`.
- **Colorful CLI**: Uses `colorama` for visually appealing output with box-drawing borders and colored icons.
- **Asynchronous Execution**: Built with `asyncio` for efficient concurrent task processing.
- **Error Handling**: Comprehensive error catching with retry logic for API failures.
- **Bilingual Support**: Supports both English and Vietnamese output.
- **Proxy Support**: Supports HTTP, HTTPS, and SOCKS5 proxies via `proxies.txt`.
- **Twitter Integration**: Auto-follow, auto-visit URLs using saved Twitter tokens.

---

### Included Scripts

✨ **Social Tasks** (`scripts/social.py`)

- ✅ Auto-scan all ecosystems & chapters for available quests
- ✅ Auto-verify quests (X Follow, Visit, and more)
- ✅ Smart ecosystem stats table with Total / Pending / Done / XP columns
- ✅ Twitter handle extraction & override mapping for onboarding quests
- ✅ Multi-account parallel execution
- ✅ Proxy support

✨ **Register + Referral + Easy Quests** (`scripts/autoreff.py`)

- ✅ Generate new EVM wallets automatically
- ✅ Sign in & join waitlist with referral code
- ✅ Turnstile captcha solving (supports 2Captcha, Anti-Captcha, CapSolver, Yescaptcha, CapMonster)
- ✅ Skip onboarding
- ✅ Auto-verify easy quests (non-Twitter)
- ✅ Save generated accounts to `accounts_afyniti.txt`
- ✅ Multi-account parallel execution
- ✅ Proxy support

✨ **Connect Twitter** (`scripts/connect.py`)

- ✅ X (Twitter) account linking via OAuth
- ✅ Auto mode (with saved tokens) & Manual mode (browser-based)
- ✅ Standard Access (full permissions for auto quests) & Restricted Access (read-only)
- ✅ Username display after successful connection
- ✅ Sequential account processing for OAuth flow
- ✅ Proxy support

✨ **Claim Equipment** (`scripts/mint.py`)

- ✅ Check claimable equipment from waitlist unlocks
- ✅ Auto-claim equipment
- ✅ Share claim to X (Twitter) for bonus XP
- ✅ Skip if already claimed/shared
- ✅ Multi-account parallel execution
- ✅ Proxy support

---

## 🛠️ Prerequisites

Before running the scripts, ensure you have the following installed:

- **Python 3.8+**
- **pip** (Python package manager)
- **Dependencies**: Install via `pip install -r requirements.txt`
- **pvkey.txt**: Add EVM private keys (one per line)
- **proxies.txt** (optional): Add proxy addresses for network requests
- **tokenX.txt** (optional): Add Twitter auth tokens (format: `auth_token|ct0`)
- **Captcha API key file** (for `autoreff.py`): Save service key in respective file (e.g., `2captchakey.txt`)

---

## 📦 Installation

1. **Clone or download this repository:**
   ```sh
   git clone https://github.com/thog9/Afyniti-social.git
   cd Afyniti-social
   ```

2. **Install Dependencies:**
   ```sh
   pip install -r requirements.txt
   ```

3. **Prepare Input Files:**

   Create `pvkey.txt` in the root directory with EVM private keys (one per line):
   ```
   0x999x999
   0x999x999
   ```

   Create `proxies.txt` (optional) — one proxy per line:
   ```
   http://user:pass@ip:port
   socks5://user:pass@ip:port
   ```

   Create `tokenX.txt` (optional) — Twitter auth tokens:
   ```
   auth_token_value|ct0_value
   ```

4. **Run:**
   ```sh
   python main.py
   ```
   - Choose a language (Vietnamese / English).
   - Select the script you want to run.

**Language Selection:**
- Choose between Vietnamese (Tiếng Việt) and English.
- All scripts support bilingual output.

---

## 📁 Project Structure

```
Afyniti-bot/
├── main.py                 # Central menu system
├── pvkey.txt               # EVM private keys
├── proxies.txt             # Proxies (optional)
├── tokenX.txt              # Twitter auth tokens (optional)
├── requirements.txt        # Python dependencies
├── README.md               # This file
└── scripts/                # Individual scripts
    ├── social.py           # Auto verify all quests
    ├── autoreff.py         # Auto register + referral + easy quests
    ├── connect.py          # Twitter OAuth connection
    └── mint.py             # Claim equipment

```

---

## 📨 Contact

Connect with us for support or updates:

- **Telegram**: [thog099](https://t.me/thog099)
- **Channel**: [CHANNEL](https://t.me/thogairdrops)
- **Group**: [GROUP CHAT](https://t.me/thogchats)
- **X**: [Thog](https://x.com/thog099)

---

## ☕ Support Us

Love these scripts? Fuel our work with a coffee!

🔗 BUYMECAFE: [BUY ME CAFE](https://buymecafe.vercel.app/)

🔗 WEBSITE: [BUY SCRIPTS](https://thogtoolhub.com/)
