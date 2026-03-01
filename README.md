# Telegram Trade Copier

Developed by **Baraka Emmanuel**  
Telegram Automation Engineer | Quantitative Forex Systems Developer  
Kampala, Uganda

---

## Overview

This repository contains a real-time Telegram to MetaTrader 5 (MT5) trade copier engineered for deterministic and low-latency signal execution.

The system listens to structured trading signals from Telegram channels, parses them using modular logic, applies configurable risk management rules, and executes trades directly through the MetaTrader 5 API.

The architecture is designed for stability, execution precision, and scalability in automated Forex trading environments.

---

## System Architecture

Telegram Channel  
→ Signal Parser (`core/signal_parser.py`)  
→ Risk Manager (`core/risk_manager.py`)  
→ Execution Engine (`core/execution_engine.py`)  
→ MetaTrader 5 API  
→ Broker  

---

## Core Features

- Asynchronous Telegram listener (Telethon)
- Intelligent signal parsing engine
- Configurable risk-per-trade model
- Deterministic MT5 execution gateway
- Slippage control logic
- Structured logging and monitoring
- External configuration via JSON
- Modular system architecture

---

## Project Structure
