# trading-platform

This project is a C++-based high-performance backtesting and live shadow trading engine, created as part of the GoQuant hiring challenge.

It reads historical price data, simulates trades using a modular strategy engine, calculates profits, and exports logs and metrics for review.

---

## 📁 Project Structure

GouantBacktester/
├── CMakeLists.txt # CMake build configuration
├── src/
│ ├── main.cpp # Core simulation engine
│ ├── strategy.h # Abstract strategy interface
│ ├── sma_strategy.h # SMA-based trading strategy
│ └── price_data.h # Price data structure
├── data/
│ └── btc_usd.csv # Sample historical data
│ └── trades.csv # Output: backtest trade log
│ └── live_trades.csv # Output: live simulation trade log
├── build/ # CMake build folder


---

## 🧠 Features

✅ SMA-based strategy  
✅ Live trading simulation  
✅ Slippage handling  
✅ Trade logging to CSV  
✅ Performance metrics:
- Sharpe Ratio
- Max Drawdown  
✅ Designed for modular strategy extension

---

## ⚙️ How to Build & Run (Beginner-Friendly)

### Prerequisites
- CMake installed (https://cmake.org/download/)
- g++ or Visual Studio compiler

---

### 🛠️ Build Steps

```bash
# Open terminal or PowerShell in the root folder

# Step 1: Generate build files
cmake -S . -B build

# Step 2: Compile the project
cmake --build build

# Step 3: Run the backtester
./build/backtester.exe
