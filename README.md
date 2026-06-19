Here’s a **complete README.md** you can copy and paste directly into your repository. It’s structured, professional, and tailored for your Gophish setup on a DigitalOcean droplet:

```markdown
# Zimparks Cybersec Gophish Setup

This repository contains configuration files, templates, and scripts for deploying and managing a **Gophish phishing simulation platform** on a **DigitalOcean droplet running Kali Linux**.

---

## 📖 Overview
Gophish is an open-source phishing framework designed for businesses, penetration testers, and security teams to run realistic phishing campaigns in a controlled environment.  
This repository organizes reusable assets and setup instructions to streamline deployment and management.

---

## ⚙️ Installation

### 1. Clone Repository
```bash
git clone https://github.com/Nyoni/zimparks-cybersec-gophish.git
cd zimparks-cybersec-gophish
```

### 2. Install Dependencies
Ensure Git and unzip are installed:
```bash
sudo apt update
sudo apt install git unzip -y
```

### 3. Download & Run Gophish
```bash
wget https://github.com/gophish/gophish/releases/latest/download/gophish-v0.12.1-linux-64bit.zip
unzip gophish-v0.12.1-linux-64bit.zip -d gophish
cd gophish
sudo ./gophish
```

---

## 📂 Repository Structure

| **Folder** | Purpose |
|-----------------|---------|
| `templates/`    | Email and landing page templates |
| `scripts/`      | Automation scripts for deployment |
| `configs/`      | Sample configuration files (without secrets) |
| `docs/`         | Documentation and usage notes |
| `.gitignore`    | Prevents sensitive files (logs, db, config.json) from being committed |

---

## 🔒 Security Notes
- Do **not** commit sensitive data (campaign results, credentials, API keys).
- `config.json` and `db/` are excluded via `.gitignore`.
- Use placeholders in templates for safe sharing.
- This repository is intended for **educational and internal security training purposes only**.

---

## 🚀 Usage
1. Customize templates in `templates/`.
2. Adjust configs in `configs/` (without secrets).
3. Run Gophish on your droplet:
   ```bash
   ./gophish
   ```
4. Access the admin panel at:
   ```
   https://your_droplet_ip:3333
   ```

---

## 📜 License
This project is for **educational and authorized security training purposes only**.  
Do not use for unauthorized phishing activities.

---

## 👨‍💻 Maintainer
- Repository owner: **Nyoni**
- Contact: tafnyoni123@gmail.com
