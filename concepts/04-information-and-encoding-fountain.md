# Concept 04.1: The Data Fountain (Information & Encoding)

A digital workbench designed to visualize the "metamorphosis" of information from human-readable text into its various numeric and algorithmic representations.

## The Visual Metaphor: "The Extrusion"
Information is treated as a physical substance. The user types at the "Now" line (the typewriter input), and as the text is produced, it is extruded into the "Past" (moving up the screen). 

- **The Present (Input):** Clear, elegant, and legible characters.
- **The Past (History):** As data moves further from the point of creation, it loses its "human skin" and reveals its "numeric skeleton."

## Core Mechanics

### 1. The Random Fade (Text to Hex)
As characters ascend, they enter a transition zone where they flicker between their character form and their Hexadecimal value.
- **Probability Logic:** The likelihood of a cell showing Hex increases with its distance (Y-index) from the input line.
- **Visual Effect:** A vibrating, "glitchy" transition that stabilizes into a solid column of Hex data in the upper reaches of the screen.

### 2. Multi-Perspective Columns
Depending on the screen real estate, the same information is shown in parallel flows:
- **Central Flow:** The Text/Hex transition. Constant-width grid where whitespace and newlines are represented as distinct symbols or empty cells rather than breaking the layout.
- **Raw Binary (The Texture):** A parallel column representing each character as an 8-bit block. High-contrast cells (filled/empty) create a unique visual texture for every string.
- **The Repacking (Base64/32):** A complex visualization showing how the 8-bit blocks are "sliced" into 6-bit or 5-bit chunks. 
    - **SVG Overlays:** Thin lines or "threads" connect the bits from the 8-bit column to their new homes in the repacked column, echoing the project's knitting/weaving theme.

## Technical Implementation (Digital Prototype)

### Frontend Stack
- **HTML/CSS Grid:** For the primary column layout and character-cell alignment.
- **Web Typography:** High-contrast monospaced fonts (e.g., JetBrains Mono) to maintain grid integrity.
- **Vanilla JavaScript:** 
    - A "Flicker Engine" to handle the random state changes of cells.
    - A reactive flow where new input "pushes" the history upwards.
- **SVG:** To draw the bit-repacking "threads" between columns.

## Goals for the Digital Medium
- Provide a "live" experience where the user can feel the weight of their data.
- Experiment with color palettes (e.g., high-contrast blueprint, dark terminal, or parchment) to prepare for physical manifestation.
- Allow for "presets" of famous text/code to demonstrate specific encoding patterns.
