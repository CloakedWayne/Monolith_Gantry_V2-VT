[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

# Monolith Gantry [WIP]

![6](Images/tensioner.png)

## What's this?
This is a performance-oriented, configurable gantry system for Voron 2.4 and Trident.

**Available drive configurations:**
- 2 stepper
- 4 stepper

**Available belt widths:**
- 6mm
- 9mm

**Available X-axis configurations:**
- Front rail (flipped belts, toothed side facing the X extrusion)
- Top rail

## What's the catch?
- You have to space out the front and rear panels on your printer by at least 5mm (Monolith Panels).
- The tensioner range is half compared to stock.
- There's limited toolhead support currently (Archetype and the Hevort version of the VZ toolhead).
- If you want to serialize your printer you have to build it stock first.
- Z chain relocation on V2.
- Trident top rail configs may need a bed relocation to get to the front of the bed (you can just move the PEI sheet for the same effect).

## DISCLAIMER: This is a challenging mod and a lot of this stuff needs further testing.

## Printed parts guide
- Recommended print settings: 4 walls, 40% infill (or more), 0.2mm layer height, 0.4mm nozzle
- Recommended material for 6mm versions: **ABS or better**
- Recommended material for 9mm versions: **ABS CF or better**
- **AB** = normal, **CD** = mirrored

### Front rail:
|Drive|Front mounts (2x)|Rear mounts (2x)|Tensioners (2x)|XY joints (L + R)|
|---|---|---|---|---|
|2 stepper|CD|AB|AB|CD|
|4 stepper|AB|AB|AB|AB|

### Top rail:
- Right front belt on top: **AB**
- Left front belt on top: **CD**

|Toolhead|Drive|Front mounts (2x)|Rear mounts (2x)|Tensioners (2x)|XY joints (L + R)|
|---|---|---|---|---|---|
|AB|2 stepper|AB|CD|CD|AB|
|AB|4 stepper|AB|AB|AB|AB|
|CD|2 stepper|CD|AB|AB|CD|
|CD|4 stepper|CD|CD|CD|CD|

If you've got any questions you can find me on Discord ***@CloakedWayne***

<br/><br/><br/><br/>
This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
