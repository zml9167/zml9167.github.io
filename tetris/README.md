# Tetris Game

A classic Tetris game developed using Godot 4.6 engine.

## Game Introduction

This is a modern implementation of the classic Tetris game, developed using Godot 4.6 engine. The game features smooth animations, multiple control methods, score system, and save functionality.

## GitHub Repository

The game source code is hosted on GitHub: [https://github.com/zml9167/tetris](https://github.com/zml9167/tetris)

## Play Online

Click here to start the game: [Tetris Game](https://zml9167.github.io/tetris/Tetris.html)

## How to Play

### Game Objectives
- Control falling blocks and arrange them into complete horizontal lines
- Completed horizontal lines will be cleared, earning points
- Prevent blocks from stacking to the top of the screen
- Try to achieve the highest score possible

### Controls

**Keyboard Controls:**
- **Left Arrow / A**: Move left
- **Right Arrow / D**: Move right
- **Down Arrow / S**: Move down (soft drop)
- **Up Arrow / W / E**: Rotate clockwise
- **Q**: Rotate counterclockwise
- **Esc**: Pause game

**Gamepad Controls:**
- **D-pad Left/Right**: Move left/right
- **D-pad Down**: Move down
- **A Button**: Rotate clockwise
- **B Button**: Rotate counterclockwise
- **Start Button**: Pause game

### Game Rules
1. Blocks fall from the top of the screen
2. Use controls to move and rotate blocks
3. Complete horizontal lines to clear them and earn points
4. Game speed increases as you level up
5. Game ends when blocks stack to the top of the screen
6. Rotation is blocked when it would cause blocks to go below the bottom boundary
7. Hold down arrow for fast drop

### Game Features
- Classic Tetris gameplay
- Keyboard and gamepad support
- Score system with level progression
- Save/Load functionality
- Pause menu
- Game over screen
- High score tracking
- Abandon run confirmation dialog
- Improved collision detection
- Smooth rotation mechanics

## Technology Stack

- **Game Engine**: Godot 4.6
- **Development Language**: GDScript
- **Graphics**: 2D Graphics
- **Deployment**: WebAssembly (WASM)

## Project Structure

```
tetris/
├── assets/          # Game assets
│   └── block.png    # Block sprite
├── prefab/          # Tetromino prefabs
│   ├── prefab0.tres
│   ├── prefab1.tres
│   └── ...
├── scene/           # Game scenes
│   ├── block/       # Block component
│   ├── global/      # Global game state
│   ├── main/        # Main game scene
│   ├── pause_menu/  # Pause menu
│   └── title/       # Title screen
├── script/          # Game scripts
│   ├── controller.gd  # Block controller
│   ├── prefab.gd      # Tetromino prefab
│   └── save_data.gd   # Save data management
├── project.godot    # Project configuration
└── README.md        # This file
```

## Local Development

1. Download and install Godot 4.6
2. Clone the repository:
   ```bash
   git clone https://github.com/zml9167/tetris.git
   ```
3. Open the project in Godot (select the `project.godot` file)
4. Click the play button to start the game

## Save and Load

- The game automatically saves your progress when you pause
- You can continue your game from the title screen
- You can abandon your current run from the title screen (with confirmation)

## Contributing

Pull Requests are welcome to improve this project!

## License

This project is licensed under the MIT License - see the LICENSE file for details.
