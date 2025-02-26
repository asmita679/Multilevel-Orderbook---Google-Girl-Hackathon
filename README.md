# AI-Driven Multilevel-Orderbook---Google-Girl-Hackathon

## Overview

This project is an AI-driven quantitative finance order book implemented in C++. It is designed for high-frequency trading environments and leverages low-latency programming techniques along with advanced object-oriented principles. The order book supports multiple order types (Market, Good-Till-Cancel, Fill-Or-Kill, etc.), efficient order matching using a price-time priority mechanism, and concurrency via multi-threading.

Potential AI integration can enhance the system by providing market predictions, optimizing order execution strategies, and detecting anomalies.

## Features

- **High-Performance Order Matching:** Implements a secure order matching engine with price-time priority.
- **Multi-Threaded Processing:** Uses mutexes and condition variables for safe, concurrent execution.
- **Multiple Order Types:** Supports Market, Good-Till-Cancel, Fill-Or-Kill, Good-for-Day, etc.
- **Extensible Architecture:** Designed for potential AI integration to further optimize trading strategies.
- **Detailed Trade Execution:** Records and processes trade information efficiently.

## Requirements

- **Compiler:** A C++17 (or later) compliant compiler (MSVC, GCC, or Clang).
- **Development Environment:**  
  - **Windows:** Visual Studio 2019/2022 (solution files provided).  
  - **Linux/macOS:** CMake is recommended.
- **Optional (for AI Integration):** ONNX Runtime (if integrating ONNX-based AI models).

## Environment Setup

### Windows (Using Visual Studio)

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/asmita679/Multilevel-Orderbook---Google-Girl-Hackathon.git
   ```

2. **Open the Solution:**
   - Open `Orderbook.sln` in Visual Studio.

3. **Configure and Build:**
   - Select your desired configuration (Debug/Release).
   - Build the solution (Build > Build Solution).

### Linux/macOS (Using CMake)

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/asmita679/Multilevel-Orderbook---Google-Girl-Hackathon.git
   ```

2. **Create a Build Directory:**

   ```bash
   mkdir build && cd build
   ```

3. **Run CMake and Build:**

   ```bash
   cmake ..
   make
   ```

## Running the Code

After building the project, run the executable as follows:

- **Windows:**
  - Navigate to the output directory (e.g., `bin/Release` or `bin/Debug`).
  - Run `Orderbook.exe`.

- **Linux/macOS:**
  - In the build directory, run:

    ```bash
    ./Orderbook
    ```

## Code Structure

- **`main.cpp`**  
  Entry point of the application.

- **`Orderbook.h` & `Orderbook.cpp`**  
  Core implementation of the order book, including order matching, cancellation, and pruning logic.

- **Order and Trade Files:**  
  Files like `Order.h`, `Trade.h`, `TradeInfo.h`, `OrderType.h`, and `OrderModify.h` define data structures and functionalities for handling orders and trades.

- **Utility and Data Files:**  
  Files such as `Usings.h`, `LevelInfo.h`, and `Constants.h` provide type definitions, level information, and constants used throughout the project.

## Testing

- **Unit Testing:**  
  Unit tests (if available) are located in the `/tests` directory.  
  Run tests using your preferred testing framework (e.g., GoogleTest).

- **Stress Testing:**  
  The project is designed to simulate high-frequency trading scenarios. Ensure that all tests pass under different market conditions before deploying.

## AI Integration

This project is designed to allow seamless integration of AI enhancements. Potential AI applications include:

- **Market Prediction:**  
  Train models (e.g., LSTM or Transformer models in Python) using historical data, export to ONNX, and integrate using ONNX Runtime.

- **Optimized Order Matching:**  
  Implement reinforcement learning models to determine the best order execution strategies under varying market conditions.

- **Anomaly Detection:**  
  Use machine learning techniques (e.g., Isolation Forests or Autoencoders) to detect and prevent fraudulent activities.
  
Our AI models are trained using TensorFlow/PyTorch and exported to ONNX format for efficient inference. The integration with C++ is achieved using **ONNX Runtime** (or TensorFlow Lite, if applicable), ensuring optimized performance and portability.  


## Contributing

Contributions are welcome! Feel free to fork this repository and submit pull requests. For major changes, please open an issue to discuss your ideas.

## Contact

For questions or further discussion, please contact [biswasasmita679@gmail.com] or visit my [GitHub Profile](https://github.com/asmita679).

---

