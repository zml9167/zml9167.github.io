# Snake Game

A classic Snake game developed using Godot 4 engine.

## Game Introduction

This is a modern implementation of the classic Snake game, developed using Godot 4 engine. The game features smooth animations, responsive controls, and modern interface design.

## GitHub Repository

The game source code is hosted on GitHub: [https://github.com/zml9167/snake](https://github.com/zml9167/snake)

## Play Online

Click here to start the game: [Snake Game](https://zml9167.github.io/snake/Snake.html)

## How to Play

### Game Objectives
- Control the snake to move and eat food to grow its body
- Avoid hitting walls or your own body
- Try to achieve the highest score possible

### Controls

**Keyboard Controls:**
- **Arrow Keys (↑ ↓ ← →)**: Control the snake's movement direction
- **WASD Keys**: Alternative to arrow keys for movement

### Game Rules
1. The snake moves forward automatically
2. When eating food, the snake's body grows and the score increases
3. Hitting walls or the snake's own body results in game over
4. As the score increases, the game speed gradually accelerates

### Game Features
- Smooth animation effects
- Responsive controls
- Score system
- Modern interface design
- Progressive difficulty increase

## Technology Stack

- **Game Engine**: Godot 4
- **Development Language**: GDScript
- **Graphics**: 2D Graphics
- **Deployment**: WebAssembly (WASM)

## Project Structure

```
snake/
├── scene/
│   ├── food/          # Food object and logic
│   ├── hud/           # Heads-up display
│   ├── main/          # Main game scene and logic
│   └── snake/         # Snake object and logic
├── .editorconfig      # Editor configuration
├── .gitattributes     # Git attributes
├── .gitignore         # Git ignore rules
├── icon.svg           # Game icon
├── project.godot      # Godot project configuration
└── README.md          # This file
```

## Local Development

1. Download and install Godot 4
2. Clone the repository:
   ```bash
   git clone https://github.com/zml9167/snake.git
   ```
3. Open the project in Godot (select the `project.godot` file)
4. Click the play button to start the game

## Contributing

Pull Requests are welcome to improve this project!

## License

This project is licensed under the MIT License - see the LICENSE file for details.
