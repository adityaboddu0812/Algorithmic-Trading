<h1 align="center">📈 Algorithmic Trading Platform</h1>

<p align="center">
  A full-stack AI-driven algorithmic trading platform with backtesting, paper trading, 
  strategy optimization, and real-time analytics.
</p>

<p align="center">
  <strong>Backend:</strong> Flask (Python) · 
  <strong>Frontend:</strong> Next.js 14 (React + TypeScript) · 
  <strong>Database:</strong> SQLite  
</p>

---

## 🔗 Live Project  
👉 [https://algorithmic-trading-fawn.vercel.app](https://algorithmic-trading-fawn.vercel.app)

---

## 🌟 Overview

This project is an end-to-end system for researching, simulating, and analyzing algorithmic crypto trading strategies.  
It includes:

- 🔐 **JWT authentication**
- 🤖 **Strategy engine** (RSI/EMA, MACD, Bollinger-RSI, custom strategies)
- 📊 **Backtesting** with equity curve, trades & performance metrics
- 🧪 **Paper trading** using live market data
- 📈 **Optimizer** (multi-strategy × multi-symbol comparison)
- 🗄️ **SQLite database** + CSV/JSON logs
- 🖥️ **Interactive dashboards** (Next.js, Tailwind, shadcn/ui)

---

## 🏛️ Architecture

```bash
Frontend (Next.js 14, TS)
│
├── Auth (JWT)
├── Dashboards & Charts
└── Calls API → Backend

Backend (Flask, Python)
│
├── Authentication
├── Backtesting Engine
├── Paper Trading Engine
├── Optimizer
├── Strategy Loader
├── Binance Data Connector
│
├── SQLite Database
└── CSV / JSON Logs

```
---

## 📂 Project Structure

```bash
Frontend/ → Next.js dashboard (TS, Tailwind, shadcn)
Backend/ → Flask REST API
Backend/strategy/ → Trading strategies
Backend/utils/ → Binance connector & helpers
Backend/logs/ → Backtests, optimizer, paper trading logs
Backend/instance/ → SQLite database (ai_trader.db)
.env.example → Environment template
docker-compose.yml → Optional Docker setup
```


---

## 🔌 Key API Endpoints

### 🔑 Authentication
```bash
POST /api/register
POST /api/login
```


### 📊 Analytics
```bash
GET /api/equity
GET /api/pnl
GET /api/trades
GET /api/positions
```


### 🔍 Backtesting
```bash
POST /api/backtest
GET /api/backtest/results
```


### 🧪 Paper Trading
```bash
POST /api/papertrading
GET /api/paper/balance
POST /api/paper/deposit
POST /api/paper/withdraw
POST /api/paper/symbol
```


### ⚡ Optimizer
```bash
POST /api/optimizer
GET /api/optimizer
```
---

## 🧪 Running the Project Locally

### ▶️ Backend (Flask)
```bash
cd Backend
pip install -r requirements.txt
python api.py
```
### ▶️ Frontend (Next.js)
```bash
cd Frontend
npm install
npm run dev
```


### 🎯 What You Can Do With This Project

- Run strategy backtests with detailed trade logs

- Visualize equity curves & performance metrics

- Compare strategies using the optimizer

- Simulate live trading safely in paper mode

- Extend or build new custom strategies

- Explore market behavior with real OHLCV data

## Developed by [Aditya Boddu](https://github.com/adityaboddu0812)

