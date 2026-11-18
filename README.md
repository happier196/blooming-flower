# Blooming flower — 3D-print files

Cleaned STL files for the six-petal, SG90-driven blooming flower with a slim stem and six linkage-aligned openings.

**[Download all printable STLs](https://github.com/happier196/blooming-flower/raw/refs/heads/main/Print_Ready_STLs.zip)**  
Or open the [individual STL files](stl/).

## What to print

There are **12 unique files and 24 printed pieces**. There are two petal designs: print three of each, then alternate inner and outer petals around the hub.

| File | Part | Quantity |
|---|---|---:|
| [01](stl/01_hex_hub_with_mounting_holes.stl) | Slotted hexagonal hub | 1 |
| [02](stl/02_inner_petal.stl) | Inner petal | 3 |
| [03](stl/03_outer_petal.stl) | Outer petal | 3 |
| [04](stl/04_connecting_rod_26mm.stl) | 26 mm head link | 6 |
| [05](stl/05_slim_stem_and_conical_connector.stl) | Combined stem and slotted cone | 1 |
| [07](stl/07_base_cup.stl) | Base cup | 1 |
| [08](stl/08_lid_with_stem_socket.stl) | Base lid and stem socket | 1 |
| [09](stl/09_adjustable_SG90_cradle.stl) | Adjustable SG90 cradle | 1 |
| [10](stl/10_servo_shim_0p9mm.stl) | Optional 0.9 mm servo shim | 1 |
| [11](stl/11_pushrod_clamp_clevis.stl) | Pushrod clamp clevis | 1 |
| [12](stl/12_servo_connecting_link_24mm.stl) | 24 mm servo link | 1 |
| [13](stl/13_glue_on_base_foot.stl) | Base foot | 4 |

Number 06 is intentionally absent: the stem and cone are combined in part 05. The total includes the optional shim.

## Before printing

- Import in **millimetres at 100% scale**. Each individual part fits within 180 × 180 × 180 mm; allow extra room for brim/support and printer exclusion zones. The stem is 167 mm tall; the base is 124 mm across.
- Select the actual printer, nozzle and material in your slicer. No printer-specific G-code is included.
- For PLA with a 0.4 mm nozzle, suggested starting settings are 0.16 mm layers for petals/joints, 0.20 mm for the base, 3 walls, 4 top/bottom layers and 20–30% infill. These are untested starting settings; use the printer's material profile.
- **Petals require supports** beneath the curved shell and suspended root. Their exported side orientation has no stable flat contact face. Inspect every layer for missing thin walls and floating starts. Keep support out of hinge holes.
- Print the stem upright with an 8–10 mm brim. Keep support out of the internal rod passage; it cannot be removed from there. Check the cone-window bridges and mounting lugs; use only accessible support.
- Print the links flat with their holes vertical, the cup open-side up, and the lid flat underside-down. Inspect small overhangs, nut pockets and cable-tie tunnels before printing.
- First print one inner petal, one outer petal, the hub, one head link and the servo cradle. Check pin movement and actual servo fit before making every copy.

All 12 exported STLs passed the [mesh audit](print-audit.json) after cleanup of tiny collapsed/duplicate faces. Dimensions are listed in [print-parts.json](print-parts.json). Physical fit, strength and servo operation remain untested.

## Not printed

Use an SG90 servo with its supplied horn, metal hinge pins, brass wire and pushrod, screws/nuts, and cable ties. The STL files do not include these hardware components.

The head was reconstructed from the visible mechanism in Jiří Praus's blooming-flower reference, with an independently designed stem and SG90 base. These are not the creator's original CAD files.
