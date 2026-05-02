# The Data Fountain (Information & Encoding)

A digital workbench designed to visualize the "metamorphosis" of information from human-readable text into its various numeric and algorithmic representations.

## The Visual Metaphor: "The Extrusion"
Information is treated as a physical substance. The user types at the "Now" line (the typewriter input), and as the text is produced, it is extruded into the "Past" (moving up the screen).

- **The Present (Row 0):** Always 100% human-readable. Clear, elegant, and legible characters.
- **The Past (History):** As data moves further from the point of creation, it loses its "human skin" and reveals its "numeric skeleton."

## Core Mechanics

### 1. Synchronized Row Flicker (Text to Hex)
The transition from character to Hexadecimal value happens at the **row level** to emphasize structural integrity.
- **Linear Probability:** 
    - Row 0: 0% Hex.
    - Row 20: 100% Hex (solidified).
    - Rows 1-19: Linear 5% increase in probability per row.
- **Rhythmic Timing:** 
    - The transition duration is exactly **1 second**, creating a slow, meditative fade.
    - The row state is re-evaluated every **1 second**.
    - All characters in a single row flip states simultaneously.

### 2. The Data Stream
- **Character-by-Character:** Extrusion happens as the user types, not on "Enter."
- **6-Byte Constraints:** Each row is exactly 6 bytes (48 bits) wide. This specific width is chosen to facilitate future Base64 (6-bit) and Base32 (5-bit) repacking visualizations.
- **Technical Symbols:** Special characters are represented by common technical editor symbols to remain visible:
    - Space: `·` (middle dot)
    - Newline: `↵` (carriage return arrow)
    - Tab: `→` (right arrow)

### 3. Multi-Perspective Columns
- **Visual Binary (Left):** A 10x3px vertical bit-texture, creating a unique "fingerprint" for every character string.
- **The Fountain (Center):** The primary Text/Hex transition grid.
- **Binary Text (Right):** Literal 8-bit strings for each character.
- **[Planned] The Repacking:** A column showing bits being re-sliced into 6-bit chunks for Base64 encoding.

## Visual Design & Accessibility
- **The "Parchment" Theme:** An off-white, high-contrast palette (`#fdfbf7` background) designed for readability and accessibility (specifically considering dyslexia).
- **Typography:** High-contrast monospaced fonts (e.g., JetBrains Mono) to maintain strict grid alignment.
- **Material Intention:** The digital prototype serves as a study for future physical pieces (print, light-sensitive paper, or CNC-engraved panels).
