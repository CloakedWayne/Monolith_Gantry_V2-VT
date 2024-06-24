[![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

# Monolith Gantry
> [!IMPORTANT]
> **This is a challenging build without a step by step build guide or documentation.**

![1](Images/V2_9mm_front_rail.png)

## What's this?
This is a performance-oriented, configurable gantry platform for Voron 2.4 and Trident.

**Available drive configurations:**
- 2WD
- AWD

**Available belt widths:**
- 6mm
- 9mm

**Available X-axis configurations:**
- Front rail (flipped belts, **toothed side facing the X extrusion = limited toolhead compatibility**)

![2](Images/Monolith.png)
> [!NOTE]
> **If you have questions or want to stay more up to date with Monolith, consider joining the dedicated Discord server.**
>
> [![Join the Discord](https://discord.com/api/guilds/1227971059764953230/widget.png?style=banner3)](https://discord.gg/JanBKxAzDz)
>
> **If you would like to see more of this and other projects in the future, consider supporting me on Ko-fi.**
>
> [![Join the Discord](https://github.com/CloakedWayne/Monolith_Gantry_V2-VT/blob/main/Images/kofi_short_button_white.png)](https://ko-fi.com/cloakedwayne)
## 2024 Roadmap
### Planned improvements for R1:
- printed and metal versions
- toothed idler delete (drive pulleys with live shafts last longer and they're easier to source with 16mm OD)
- significant effective tensioner range increase (50% or more)
- optional zero protrusion mode (no extra panel spacing, but similar build volume loss to other AWDs) without changing the gantry parts

## Design goals
- The shortest and the simplest belt path possible without losing full bed capability even with AWD (toolhead dependant)
- AWD without increasing belt length and idler count
- Double shear support
- Increased printed part rigidity
- Uncluttered design
- Cheap BOM

## Performance expectations
**2WD:** Due to the 10-15cm shorter belt path, stiffer and lighter XY joints (inside Y rails) your printer should perform similarly to a 50mm smaller one equipped with the same toolhead and X axis setup.

**AWD:** It doesn't come at the cost of adding 20cm extra belt length and more idlers, so input shaper scaling should be close to +100% vs 2WD due to the truly halved effective belt length. IF there are no rigidity bottlekecks elsewhere, which is rarely the case.

## What's the catch?
- **There's limited toolhead support currently because of the flipped belt path.** Voron-compatible toolheads that have loop-around belt clips will work, but you WILL lose the ability to tuck away the excess belt.
- You have to space out the front (AWD only) and rear panels on your printer by at least 5mm ([Monolith Panels](https://github.com/CloakedWayne/Monolith_Panels)) or have a 4040 frame.
- The tensioner range is less than half compared to stock. Monolith is not recommended for larger than 350mm build volume.
- Z chain relocation/delete on V2
- Trident rear vertical extrusion brackets have to be rotated by 180 degrees

<br/><br/><br/><br/>
This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
