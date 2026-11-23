 <p align="center">
  <img src="crimgif.gif" alt="Crim+ Mascot - Crimson" width="220" />
</p>

<h1 align="center">Crim+ (v1.6.0)</h1>

<p align="center">
  <strong>"Create scripts the way you think."</strong><br/>
  A plain-English scripting language and 2D game engine built to bridge the gap between Scratch and Python.
</p>

<p align="center">
  <a href="https://github.com/CrimsonCyan-CODE/Crim-PLUS/releases/latest"><strong>⬇️ Download Crim+ for Windows</strong></a> •
  <a href="https://crimsoncyan-code.github.io/CrimIDE"><strong>🌐 Web IDE (Some features are unsupported in the Website, try other langs too!)</strong></a>
</p>

---

## Why Crim+?

Jumping straight from visual blocks in Scratch to Python syntax can be overwhelming for young coders. **Crim+** lets kids and beginners write real, text-based 2D games that read like storytelling — while still packing enough power to build complete, rule-heavy games like a **full Chess engine with PGN export**.

- **Plain-English Syntax:** Write natural commands like `when the tilemap is clicked, do:`, `plug tilemap to display`, and `give back`.
- **Built-in 2D Engine:** Powered by Pygame, targeting 60 FPS, with sprites, shapes, tilemaps, text, WAV audio, and collision events.
- **Standalone Runtime:** Crim+ includes its own runtime. No separate Python installation or configuration is required.
- **ROSE Package Manager:** Install and share community modules directly from your terminal.
- **CDSL Support:** Includes a custom data serialization format built specifically for Crim+ projects.

---

## What Crim+ Code Looks Like

Here is a real snippet from a **complete Chess game** built in Crim+ (complete with legal move validation, castling, *en passant*, checkmate detection, and `.pgn` match export):

```crim
use tilemap
use display

display width is 480
display height is 480
display background is "chessboard.png"
open display

# Connect a 60x60 tilemap grid to the window
plug tilemap to display, tile size is 60 pixels

# Handle mouse clicks on the board
when the tilemap is clicked, do:
    set destination_x to mouse tile x
    set destination_y to mouse tile y

    if destination_x >= 0 and destination_x < 8, then do:
        set clicked to board[destination_y * 8 + destination_x]
        if clicked starts with turn, then do:
            set piece to clicked
            set x of selector to destination_x * 60
            set y of selector to destination_y * 60
            set opacity of selector to 35%
        end if
    end if
end when
```

---

## Quick Start

### 1. Install Crim+

1. Visit the **[latest Crim+ release](https://github.com/CrimsonCyan-CODE/Crim-PLUS/releases/latest)**.
2. Download the Windows installer.
3. Run the **Crim+ Setup Wizard** and follow the installation instructions.

Crim+ includes its own runtime, so you don't need to install Python separately.

### 2. Run Your First Script

Open Command Prompt, navigate to the folder containing your `.crim` file, and run:

```bash
crim my_game.crim
```

That's it! Your Crim+ script is ready to run.

---

## Using ROSE (Package Manager)

Crim+ comes with **ROSE**, its package manager for installing and creating reusable modules.

```bash
# Install a module
rose install module_name

# View available modules
rose list

# Package your own script into a module
rose cm "my_module.crim"
```

### Available Modules

Crim+ supports community modules that extend the language with additional functionality.

Some examples include:

- **mathtools** — Additional mathematical functions and utilities.
- **texttools** — Extended text manipulation and formatting.
- **csv** — CSV data parsing and handling.
- **runner** — Run Crim+ scripts through the command line.

Check the repository for available modules and updates.

---

## Platform Support

| Platform | Support |
|---|---|
| Windows | Supported |
| Linux | Not currently supported |
| macOS | Not currently supported |

Crim+ is currently distributed for Windows.

---

## License

Crim+ is open-source software released under the **MIT License**. See [LICENSE](LICENSE) for details.

---

<p align="center">
  <strong>Crim+ — Create scripts the way you think.</strong>
</p>
