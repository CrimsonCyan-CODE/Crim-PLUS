# Crim+

**Crim+** is a custom, English-like scripting language and 2D game engine built in Python using Pygame. It was designed to make coding games as easy as writing a story,
and to bridge the large gap between Python and Scratch to make text-based coding more accessible to young children that have learnt Scratch.

The interpreter (`crim.py`) reads `.crim` files and executes them line-by-line, handling graphics, math, loops, functions, and collision detection.

## Features
- **Readable Syntax:** Write code that looks like plain English (e.g., `say "Hello!"`, `if mycat touches coin, then do:`).
- **Pygame Engine:** Renders shapes, images, and text at 60 FPS.
- **Events & Collisions:** Built-in `when ... touches` and `when [key] is held` events.
- **Math:** Supports `+ - * / ^`, `sqrt`, `sin`, `cos`, `tan`, and random number generation.
- **Audio:** Play `.wav` sound effects.

## Requirements
Crim+ requires Python 3 and Pygame.
## How To Download And Use Crim+
1. Get Python from https://www.python.org/downloads
2. Open your command prompt, and use pip to install pygame:
```bash
pip install pygame
```
(Didnt work? instead try to download pygame-ce (pygame community edition, which they use to keep pygame up-to-date for new updates!)
```bash
pip install pygame-ce
```
Now, you can run crim.py (the interpreter!) Just clicking on the file wont work. Heres how to run the interpreter:
1. Open your command prompt. Lets say, as an example, that the interpreter and your Crim+ script is in your downloads.
2. Type this:
```bash
cd C:/Users/YOURUSERNAME/Downloads
```
3. Your all set! Just type:
```bash
python crim.py MyScript.crim
```
## EXTRA NOTE!
Wanna see some examples of code from me? Heres how you can run spacecat or catformer!
1. Make sure you have Python, Pygame (or Pygame-CE) and crim.py
2. Go to the latest release, and download them there!
3. Just simply open Command Prompt, and type:
```bash
python crim.py spacecat.crim
```
or
```bash
python crim.py catformer.crim
```
