# Telegram to MT5 Execution Architecture

## Execution Flow

1. Telegram Listener receives raw message
2. SignalParser extracts structured trade data
3. RiskManager calculates lot size based on equity
4. ExecutionEngine validates:
   - Symbol
   - Slippage
   - Spread
5. Order sent to MetaTrader 5 API
6. Confirmation logged

---

## Deterministic Principles

- No execution without full parameter validation
- Risk per trade capped
- Slippage threshold enforced
- Structured failure handling

---

## Latency Optimization

- AsyncIO event loop
- Persistent MT5 connection
- Preloaded symbol cache
