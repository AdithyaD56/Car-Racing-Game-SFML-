# Car-Racing-Game-SFML-

# 🚗 Car Racing Game (SFML)

A simple 2D car racing simulation game built using C++ and [SFML (Simple and Fast Multimedia Library)](https://www.sfml-dev.org/). It features AI-controlled opponent cars navigating through predefined checkpoints and a player-controlled car with realistic physics for steering and acceleration.

## 🎮 Game Features

- 2D top-down car racing.
- Player-controlled car using arrow keys.
- AI opponent cars automatically follow the track via checkpoints.
- Collision detection between cars.
- Smooth car movement with acceleration, deceleration, and turning physics.

## 🖼️ Screenshots

> Add your gameplay screenshots here (e.g., `/images/screenshot1.png`)

## 🛠️ Requirements

- C++17 or higher
- [SFML 2.5+](https://www.sfml-dev.org/download.php)
- Compatible compiler (e.g., g++, MSVC)

## 📁 Project Structure

CarRacingGame/
│
├── images/
│ ├── background.png # Race track background
│ └── car.png # Car sprite
│
├── main.cpp # Game source code
├── README.md # Project documentation


---

## ⌨️ Controls

| Key        | Action               |
|------------|----------------------|
| Up Arrow   | Accelerate           |
| Down Arrow | Brake / Reverse      |
| Left Arrow | Turn Left            |
| Right Arrow| Turn Right           |

---

## 🔄 Gameplay Mechanics

- The player's car is the **first car (index 0)** in the array.
- AI cars steer towards checkpoints using trigonometry (`atan2`, `sin`, `cos`).
- Each AI car advances to the next checkpoint once close enough.
- Basic collision logic is used to prevent overlap between cars.
- The camera follows the player's car using background offset.

---

## 🚧 How to Compile & Run

### 🐧 Linux / macOS:

```bash
g++ main.cpp -o CarGame -lsfml-graphics -lsfml-window -lsfml-system
./CarGame

🪟 Windows (MinGW or Visual Studio):
Install SFML.

Link these SFML libraries:

sfml-graphics

sfml-window

sfml-system

Ensure the images/ folder is in the same directory as the .exe.

Compile and run using your IDE or command line.

📜 License
This project is licensed under the MIT License – free to use, modify, and share!
