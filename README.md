# Deribit API Trading System (Quant Trade) in C++

This project is a trading system built in C++ for interacting with the Deribit Test API. It allows you to place, cancel, modify orders, view the order book, and retrieve current position details on the Deribit platform(https://test.deribit.com/). The project uses `cURL` for HTTP requests and `nlohmann/json` for JSON parsing.

## Features

- **Order Placement**: Submit orders at specific price and quantity for various instruments.
- **Order Management**: Cancel and modify existing orders.
- **Order Book Retrieval**: View detailed order book data including bids, asks, and market information.
- **Position Details**: Retrieve position details for a specific instrument.

## Requirements

- **C++ Compiler**: GCC (recommended) or any modern C++ compiler with C++11 support.
- **cURL**: Library for HTTP requests.
- **JSON for Modern C++**: Header-only library for JSON parsing by `nlohmann/json`.

## Dependencies

1. **cURL**: Install via the following commands:
    ```bash
    sudo apt update
    sudo apt install libcurl4-openssl-dev
    ```

2. **JSON for Modern C++**: Download the header file from [nlohmann/json GitHub page](https://github.com/nlohmann/json) or install via a package manager:
    ```bash
    sudo apt install nlohmann-json3-dev
    ```



2. Ensure the necessary libraries (`curl` and `nlohmann/json`) are installed.

3. Add the path to `json.hpp` if it's not already in your include path:
    - Place `json.hpp` in the `include/` directory within the project.

## Compilation

Use the following command to compile the project:

g++ main.cpp -o Quant_Trade -Iinclude -Iinclude/include2 -Linclude/lib -lcurl -lws2_32 -lwldap32

Run the Compiled binary : .\Quant_Trade 


