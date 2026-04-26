# Project README

## Overview
The project is a simple GUI application built using C programming language. It demonstrates wave propagation and includes basic graphical interface functionalities.

## Features
- Basic GUI for visualizing wave propagation.
- Wave propagation simulation based on user inputs.

## Project Structure
```
Gui_WavePropagation/
├── build/              # .exe files produced by Main.c
├── src/                # Source code directory
│   ├── Main.c          # Entry point of the application
│   └── wave_propagation.h  # Header file for wave propagation functions
├── Makefile.linux      # Linux Build configuration
├── Makefile.windows    # Windows Build configuration
├── Makefile.wine       # Wine Build configuration
├── Makefile.web        # Emscripten Build configuration
└── README.md           # This file
```

### Prerequisites
- C/C++ Compiler and Debugger (GCC, Clang)
- Make utility
- Standard development tools

## Build & Run
### Linux
1. Navigate to the project directory:
   ```sh
   cd Gui_WavePropagation/
   ```
2. Build the project:
   ```sh
   make -f Makefile.linux all
   ```
3. Execute the built application:
   ```sh
   ./build/Main
   ```

### Windows
1. Navigate to the project directory:
   ```sh
   cd Gui_WavePropagation/
   ```
2. Build the project:
   ```sh
   make -f Makefile.windows all
   ```
3. Execute the built application:
   ```sh
   build\Main.exe
   ```

### Wine (Linux Cross Compile for Windows)
1. Navigate to the project directory:
   ```sh
   cd Gui_WavePropagation/
   ```
2. Build the project:
   ```sh
   make -f Makefile.wine all
   ```
3. Execute the built application using Wine:
   ```sh
   wine build\Main.exe
   ```

### Web Assembly (Emscripten)
1. Navigate to the project directory:
   ```sh
   cd Gui_WavePropagation/
   ```
2. Build the project:
   ```sh
   make -f Makefile.web all
   ```
3. Serve and run the application using Emscripten's built-in server:
   ```sh
   emrun --no_browser --port 8080 build/index.html
   ```

Note: Ensure you have the required libraries installed on your system for each platform before attempting to compile the project.