## Sudoku Gladiators – Multiplayer Sudoku Game

**Sudoku Gladiators** is a cross-platform multiplayer game designed to bring the classic single-player Sudoku experience into the $21^{st}$ century. Built with **Flutter** and **Firebase**, it features ranked matchmaking, casual co-op modes, and a unique powerup system.

---

### 📖 Project Documentation

For a detailed breakdown of the project’s motivation, competitive analysis, and algorithmic implementation, please see the **[Sudoku Gladiators Presentation.pdf](./Sudoku%20Gladiators%20Presentation.pdf)**.

This document provides in-depth information on:

* 
**The "Why"**: Personal motivation and the desire to play with friends remotely.


* 
**Competitive Landscape**: Analysis of existing web apps like UsDoku and academic research like SudoDuel.


* 
**Architecture**: A deep dive into the serverless approach using Firebase transactions.


* 
**Algorithm**: Step-by-step logic for randomized backtracking and unique solution validation.



---

### 🚀 Key Features

* 
**Ranked Queue**: Competitive play featuring Elo-based matchmaking.


* 
**Casual Modes**: Includes $1 \vee 1$ on the same board, co-op modes, and powerup modes.


* 
**Unique Powerup System**: Players fight for powerups at random intervals that can affect the opponent's board.


* 
**Cross-Platform**: A single codebase for mobile, web, and desktop.



---

### 🛠️ Technical Architecture

Unlike many competitors that use custom Node.js servers and WebSockets, Sudoku Gladiators utilizes a **serverless approach**.

#### Tech Stack

* 
**Frontend**: [Flutter](https://www.google.com/search?q=https://flutter.dev/) & [Dart](https://www.google.com/search?q=https://dart.dev/).


* 
**Backend**: [Firebase](https://www.google.com/search?q=https://firebase.google.com/) for authentication, real-time database, and cloud storage without server infrastructure management.


* 
**State Management**: Uses 4 Change-Notifier providers: **Sudoku**, **Powerup**, **Theme**, and **Lobby**.


* 
**Synchronization**: Leverages Firebase **transactions** for multiplayer sync and claiming victory.



#### The Sudoku Algorithm

The game ensures high-quality, solvable puzzles through a two-step process:

1. 
**Generation**: Uses randomized backtracking with shuffled candidates [1–9] to fill a grid while validating Sudoku constraints.


2. 
**Reduction**: Randomly removes 35–55 cells and verifies that exactly one unique solution remains; if not, the cell is restored.



---

### 🔮 Future Work

* [ ] Audio effects and custom themes.


* [ ] In-depth Friend System and Tournaments.


* [ ] AI for practice modes and move suggestions.


* [ ] General bug fixing.


---
Created by **Dumitrescu David-Ioan**.
