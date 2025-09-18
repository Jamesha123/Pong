# Pong Game

A classic Pong game implementation using Java Swing and AWT frameworks. This project features a two-player Pong game with enhanced controls and modern Java module system.

## Features

- **Two-player gameplay** - Compete against a friend locally
- **Enhanced controls** - Player 1 can move in all directions (W/A/S/D), Player 2 uses arrow keys
- **Modern Java implementation** - Built with Java modules and Swing/AWT
- **Cross-platform** - Runs on any system with Java installed
- **Executable JAR** - Easy to distribute and run

## Game Controls

### Player 1 (Blue Paddle) Secret Controls
- **W** - Move up
- **S** - Move down  
- **A** - Move left
- **D** - Move right

### Player 2 (Pink Paddle)
- **↑** - Move up
- **↓** - Move down

## How to Play

1. Launch the game using one of the methods below
2. First player to reach 5 points wins
3. The ball bounces off paddles and top/bottom walls
4. If the ball goes past a paddle, the opponent scores

## Building and Running

### Prerequisites
- Java 11 or higher
- No additional dependencies required

### Quick Start (Using Pre-built Executable)
1. Download the `PongGame.jar` file
2. Double-click `PongGame.jar` or run:
   ```bash
   java -jar PongGame.jar
   ```

### Building from Source
1. Clone or download this repository
2. Compile the source code:
   ```bash
   javac -d bin src/*.java
   ```
3. Create the executable JAR:
   ```bash
   jar cfm PongGame.jar MANIFEST.MF -C bin .
   ```
4. Run the game:
   ```bash
   java -jar PongGame.jar
   ```

### Windows Users
- Use the provided `run_pong.bat` script for easy launching
- Simply double-click the batch file to start the game

## Project Structure

```
Pong/
├── src/
│   ├── PongGame.java      # Main entry point
│   ├── GameFrame.java     # JFrame window setup
│   ├── GamePanel.java     # Main game logic and rendering
│   ├── Ball.java          # Ball physics and rendering
│   ├── Paddle.java        # Paddle controls and rendering
│   ├── Score.java         # Score display and tracking
│   └── module-info.java   # Java module configuration
├── bin/                   # Compiled class files
├── PongGame.jar          # Executable JAR file
├── MANIFEST.MF           # JAR manifest
├── run_pong.bat          # Windows batch script
└── README.md             # This file
```

## Technical Details

- **Framework**: Java Swing/AWT
- **Module System**: Java 9+ modules
- **Game Loop**: 60 FPS target
- **Window Size**: 1000x556 pixels
- **Ball Speed**: Increases with each paddle hit

## Development

The game uses a modular architecture with separate classes for different game components:
- `GamePanel` handles the main game loop and collision detection
- `Ball` manages ball physics and movement
- `Paddle` handles player input and paddle movement
- `Score` displays the current score and center line

*Enjoy playing Pong! 🏓*
