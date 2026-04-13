# Hub Cost Analyzer — Demo

A web-based demo showcasing the Hub Cost Analysis system for monitoring Housekeeping, Electricity, and Tea/Coffee/Water costs across hub locations.

## 🔗 Live Demo

**[View Demo →](https://YOUR_USERNAME.github.io/hub-cost-demo/)**

### Demo Credentials
- **Email:** `admin@hub.com`
- **Password:** `demo123`

## 📊 Features

### HK & Electricity Analysis
- 15-column numeric format with category split (HK Actual vs Peer, Elec Actual vs Peer)
- Peer-based comparison using cost per sq.ft (same city)
- Self-avg fallback when no peers exist (last 3 months)
- Month-specific fraud flags: **Dup**, **Spike**, **Top**, **AboveAvg**
- Risk Score 0-10 with color coding

### TCW (Tea/Coffee/Water) Analysis
- Peer-based comparison using cost per head (DAU)
- Budget-based flags from SOP tier pricing
- 6 fraud checks: **Exceeds**, **High**, **VeryLow**, **Dup**, **Spike**, **AboveAvg**
- Self-avg fallback for hubs with no city peers

### Summary Reports
- Report 1: Flagging Wise (Low / Normal / High / Exceeds bands)
- Report 2: Status Wise (Saving vs Overspending counts + amounts)
- Report 3: Category Wise Overspend MoM (HK / Electricity split)

## 🚀 Deploy to GitHub Pages

1. Create a new repository on GitHub
2. Push this folder:
   ```bash
   cd hub-cost-demo
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/hub-cost-demo.git
   git push -u origin main
   ```
3. Go to **Settings → Pages → Source → Deploy from branch → main → / (root)**
4. Your demo will be live at `https://YOUR_USERNAME.github.io/hub-cost-demo/`

## 📁 Files

| File | Description |
|------|-------------|
| `index.html` | Login page with demo credentials |
| `dashboard.html` | Dashboard with metrics, charts, HK table, TCW table |
| `README.md` | This file |

## 🔒 Note

This is a **static demo** with sample data. The actual analysis runs as Google Apps Scripts on Google Sheets with real transaction data. The demo credentials are for preview purposes only — no real data is exposed.
