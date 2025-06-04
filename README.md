# Brick Breaker Game

A classic console-based Brick Breaker game implemented in C for Windows systems. Break all the bricks with your ball and paddle to win!

## Team Members
- **Asjad**
- **Abubakar** 
- **Rabia**

## Features

- **Two Difficulty Levels**: Easy and Hard modes with different ball speeds
- **Dynamic Paddle**: Paddle size increases as you score more points
- **Pause/Resume Functionality**: Press 'P' to pause or resume the game
- **Score System**: Earn points by breaking bricks
- **Smooth Gameplay**: 60 FPS rendering for smooth ball movement
- **Win/Lose Conditions**: Win by breaking all bricks, lose if ball reaches bottom
- **Console Graphics**: ASCII-based graphics using Windows Console API

## Game Controls

| Key | Action |
|-----|--------|
| `A` | Move paddle left |
| `D` | Move paddle right |
| `P` | Pause/Resume game |

## Game Rules

1. Use the paddle to bounce the ball and break bricks
2. Don't let the ball fall below the paddle
3. Break all bricks to win the game
4. Your paddle grows larger as you score more points:
   - Score 15: Paddle size increases to 11
   - Score 30: Paddle size increases to 12
   - Score 45: Paddle size increases to 13
   - Score 60: Paddle size increases to 14
   - Score 80: Paddle size increases to 15

## Installation & Setup

### Prerequisites
- Windows operating system
- GCC compiler (MinGW recommended)
- Windows.h library support

### Compilation
```bash
gcc -o brick_breaker brick_breaker.c
```

### Running the Game
```bash
./brick_breaker.exe
```

## Difficulty Levels

- **Easy (0)**: Slower ball speed for beginners
- **Hard (1)**: Faster ball speed for experienced players

## Technical Details

### Game Specifications
- **Screen Resolution**: 80x24 characters
- **Frame Rate**: ~60 FPS
- **Paddle Size**: Dynamic (starts at 10, grows with score)
- **Brick Layout**: 5 rows with strategic spacing

### Key Functions
- `setup()`: Initializes game state and difficulty settings
- `moveBall()`: Handles ball physics and collision detection
- `drawMap()`: Renders the game screen
- `handleInput()`: Processes player input
- `updateMap()`: Updates game state each frame

### Windows API Usage
- Console manipulation for smooth graphics
- High-precision timing for consistent frame rate
- Cursor management for clean display

## Game Architecture

The game uses a simple game loop with the following components:
1. **Input Handling**: Processes keyboard input for paddle movement and pause
2. **Game Logic**: Updates ball position, collision detection, score tracking
3. **Rendering**: Draws the game state to console buffer
4. **Timing**: Maintains consistent 60 FPS gameplay

## Screenshots/Demo

```
################################################################################
# Score: 42                     Press 'P' to pause                             #
#                                                                              #
# ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ #
#                                                                              #
# ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ #
#                                                                              #
# ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ ██ #
#                                                                              #
#                                    o                                         #
#                                                                              #
#                                                                              #
#                                                                              #
#                                                                              #
#                                                                              #
#                                                                              #
#                                                                              #
#                                                                              #
#                                                                              #
#                                                                              #
#                                                                              #
#                                                                              #
#                                                                              #
#                              ██████████████                                  #
################################################################################
```

## Known Issues & Limitations

- Windows-only compatibility due to Windows.h dependencies
- Console-based graphics limit visual appeal
- No sound effects or music
- Fixed screen resolution (80x24)

## Future Enhancements

- [ ] Cross-platform compatibility (Linux/Mac support)
- [ ] Power-ups and special bricks
- [ ] Multiple levels with different layouts
- [ ] High score system with file persistence
- [ ] Sound effects and background music
- [ ] Improved graphics with colors
- [ ] Multiple balls feature

## Contributing

This project was developed as a team effort. If you'd like to contribute:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly on Windows
5. Submit a pull request

## License

This project is open source and available under the MIT License.

## Acknowledgments

- Thanks to all team members for their contributions
- Inspired by the classic Atari Breakout game
- Built using Windows Console API for graphics rendering

---

**Enjoy breaking those bricks!** 🧱⚾