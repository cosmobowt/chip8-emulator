# CHIP-8 Emulator

A fully-featured CHIP-8 Emulator written in C++ with SDL2 for graphics and input.  
Implements the full instruction set, memory model, timers, stack, display, and keypad—faithfully recreating classic CHIP-8 games like **Pong**, **Tetris**, **Space Invaders**, and more.


## 🛠️ Build Instructions

1. **Compile using g++:**
    ```sh
    g++ Main.cpp Chip8.cpp Platform.cpp -lSDL2 -std=c++17 -o chip8
    ```
2. **▶️ Running the Emulator:** Example
    ```sh
    ./chip8 10 2 ../Tetris.ch8
    ```
## Parameters

Scale → How large each CHIP-8 pixel is (10 = 640×320 window)
CycleDelay_ms → Delay between CPU cycles (2–5 ms recommended)
ROM_File → Path to .ch8 file

## ✨ Features

- ✔️ Full CHIP-8 instruction set (all 35 opcodes)  
- ✔️ Function pointer–based opcode dispatch  
- ✔️ 4 KB memory, 16 registers, 16-level stack  
- ✔️ Built-in hexadecimal fontset (0–F)  
- ✔️ Accurate timers (delay & sound)  
- ✔️ 64×32 monochrome display buffer  
- ✔️ SDL2-based rendering & keyboard input  
- ✔️ Works with any valid CHIP-8 ROM  

---

## 📁 Project Structure
-├── Chip8.cpp # CHIP-8 CPU + Opcode Handling
-├── Chip8.hpp
-├── Platform.cpp # SDL2 Rendering + Input Layer
-├── Platform.hpp
-├── Main.cpp # Main Loop (load → run → render)
-└── README.md


