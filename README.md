# Yu-Gi-Oh! C++ Simulation 🃏

![C++](https://img.shields.io/badge/Language-C++17-blue)
![OOP](https://img.shields.io/badge/Architecture-Object_Oriented-green)
![Status](https://img.shields.io/badge/Status-Project_Completed-brightgreen)

A robust console-based simulation of the Yu-Gi-Oh! card game, built using advanced C++ Object-Oriented Programming principles. This project was developed as part of a University course (FMI) to demonstrate polymorphism, dynamic memory management, and clean code architecture.

## 🚀 Key Features

*   **Polymorphic Architecture:** Handles different card types (`Monster`, `Spell`, `Trap`, `Pendulum`) using virtual functions and inheritance.
*   **Memory Management:** Implements the "Rule of 3" (and Rule of 5 concepts) to ensure safe deep copies and prevent memory leaks.
*   **Dynamic Duel Board:** Manage zones (Monster/Backrow) and a dynamic graveyard with automatic resizing capabilities.
*   **Game Logic:** Advanced `dynamic_cast` usage to distinguish card types at runtime and handle unique play mechanics (e.g., Pendulum Scale vs. Monster).

## 🛠 Project Structure

```text
.
├── main.cpp          # Entry point and test scenarios
├── DuelBoard.h       # Game board logic and memory management
├── Card.h            # Base Card class (Abstract)
├── MonsterCard.h     # Inherits from Card
├── SpellCard.h       # Inherits from Card
└── PendulumCard.h    # Hybrid inheritance (Monster + Spell)