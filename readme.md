<p align="center">
  <img src="crimgif.gif" width="200" alt="Crim+ logo"> <--- Crimson, Crim+'s Mascot! :)
</p>

# Crim+!

(NOTE: I do know that the files all have different versions. Github is 1.4, Previous python interpreters are 0.2.4 or somethin and the setup installer says 0.27, this will be fixed soon!!!)

**Crim+** is a custom, English-like scripting language and 2D game engine built in Python using Pygame. It was designed to make coding games as easy as writing a story,
and to bridge the large gap between Python and Scratch to make text-based coding more accessible to young children that have learnt Scratch.

The setup wizard installs the interpreter that executes them line-by-line, handling graphics, math, loops, functions, and collision detection.

## Features
- **Readable Syntax:** Write code that looks like plain English (e.g., `say "Hello!"`, `if mycat touches coin, then do:`).
- **Pygame Engine:** Renders shapes, images, and text at 60 FPS.
- **Events & Collisions:** Built-in `when ... touches` and `when [key] is held` events.
- **Math:** Supports `+ - * / ^`, `sqrt`, `sin`, `cos`, `tan`, and random number generation.
- **Audio:** Play `.wav` sound effects.
- **CDSL:** A custom data serialization language meant for Crim+.
- **ROSE:** A package manager used to install modules for better experience using Crim+.

## Requirements
Crim+ requires Windows. Thats all! Originally, a python interpreter was required, but I've built a custom setup wizard!

## How to run Scripts
First, open your command prompt and set your directory to where your script is!
Then, just type:
```bash
crim script.crim
```
## Rose?
Rose is a package manager included in the Crim+ Setup Wizard that is used to install modules and create modules using Crim+ scripts.
To install a module, use this:
```bash
rose install module
```
To see a list of modules, do this:
```bash
rose list
```
To create a module, do this:
```bash
rose cm "crimscript.crim"
```
