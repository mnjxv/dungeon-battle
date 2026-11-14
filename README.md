# Dungeon Battle

A turn-based dungeon battle game for the terminal, written in pure C++17 with no external libraries.

Fight monster after monster, grow stronger with every victory, and see how many rooms you can survive.

## Features

- Turn-based combat with random damage and a 15% critical hit chance
- Four actions: **Attack**, **Defend** (halves damage), **Use potion** (+25 HP), **Run away** (50% chance)
- Five monster types that get tougher each room
- Level-ups after every victory (more HP and damage)
- Random potion drops
- Works on Windows, macOS and Linux

## How to play

Type the number of your action and press Enter.

| Key | Action |
|-----|--------|
| 1 | Attack the monster |
| 2 | Defend (take half damage this turn) |
| 3 | Drink a potion and recover 25 HP |
| 4 | Try to run to the next room |

The game ends when your HP reaches 0.

## Build and run

You only need a C++ compiler that supports C++17 (g++, clang++ or MSVC).

### Quick way

- **Windows:** double-click `build.bat`, then run `dungeon.exe`
- **macOS / Linux:** run `./build.sh`, then `./dungeon`

### Manual way

```
g++ -std=c++17 -O2 src/main.cpp -o dungeon
./dungeon
```

On Windows PowerShell, run `.\dungeon` instead.

### With make

```
make
make run
```

### Using VS Code

1. Open this folder in VS Code and install the **C/C++** extension.
2. Open the terminal (Ctrl+`) and use any of the build commands above.

### No compiler installed?

Paste the contents of `src/main.cpp` into a free online C++ compiler such as OnlineGDB or Programiz and press Run.

## Project structure

```
dungeon-battle/
├── src/main.cpp    # the whole game
├── Makefile
├── build.sh        # macOS / Linux build script
├── build.bat       # Windows build script
├── LICENSE
└── README.md
```

## Ideas for improvement

- Add a shop between rooms
- Add magic spells or different hero classes
- Add a boss every 5 rooms
- Save a high score to a file

## License

MIT License. See [LICENSE](LICENSE).
