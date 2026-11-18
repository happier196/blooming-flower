# Blooming flower — proportionally smaller 27 cm version

The **complete flower head, petals, hinge mechanism and cone are 75% of their original size in all three dimensions**. The stem is slimmer and shorter, and the pot is narrower while retaining its 6.5 cm height. Pin/screw fits and the SG90 remain sized for real hardware.

| Measurement | Original | Current |
|---|---:|---:|
| Closed height, including feet | 35.64 cm | 26.78 cm |
| Maximum height across 61 poses | — | 26.83 cm |
| Fully open flower width | 23.53 cm | 17.65 cm |
| Pot diameter | 12.4 cm | 9.6 cm |
| Pot body height | 6.5 cm | 6.5 cm |
| Cone top diameter | 4.1 cm | 3.075 cm |
| Stem diameter | 0.8 cm | 0.6 cm |

**[Download all current STLs](https://github.com/happier196/blooming-flower/raw/refs/heads/main/Print_Ready_STLs.zip)** · [Individual parts](stl/)

## Blender animation

**[Download the animated Blender model](https://github.com/happier196/blooming-flower/raw/refs/heads/main/Proportional_27cm_Flower.blend)**. Save the file and open it in Blender. Select the **COMPLETE_FLOWER** scene, place the pointer over the 3D viewport and press **Space** to play or pause the opening-and-closing loop.

The animation runs from frame **1 (closed)** through **61 (open)** to **121 (closed again)** at 30 fps. **FLOWER_HEAD_CLOSEUP** shows the head mechanism; **BASE_DRIVE_DETAIL** shows the servo linkage. **PRINT_PARTS** contains one example of each unique printable part; use the quantities below when printing.

## Print quantities

There are **12 unique files and 24 pieces**, including the optional shim. Print three of each petal design and alternate them around the hub. Number 06 is omitted because the stem and cone are one part.

| Part | Quantity | STL size, mm |
|---|---:|---|
| [Slotted hexagonal hub](stl/01_hex_hub_with_mounting_holes.stl) | 1 | 32.8 × 32.0 × 6.9 |
| [Inner petal](stl/02_inner_petal.stl) | 3 | 32.0 × 84.1 × 38.0 |
| [Outer petal](stl/03_outer_petal.stl) | 3 | 32.0 × 85.3 × 40.5 |
| [19.5 mm head link](stl/04_connecting_rod_19p5mm.stl) | 6 | 3.4 × 22.9 × 1.5 |
| [Combined 6 mm stem and slotted cone](stl/05_slim_stem_and_conical_connector.stl) | 1 | 30.8 × 30.8 × 107.8 |
| [Base cup](stl/07_base_cup.stl) | 1 | 96.0 × 96.0 × 65.0 |
| [Base lid with 6.4 mm stem socket](stl/08_lid_with_stem_socket.stl) | 1 | 96.0 × 96.0 × 17.0 |
| [SG90 cradle](stl/09_adjustable_SG90_cradle.stl) | 1 | 50.0 × 38.0 × 19.0 |
| [Optional servo shim](stl/10_servo_shim_0p9mm.stl) | 1 | 23.5 × 26.0 × 0.9 |
| [Pushrod clamp clevis](stl/11_pushrod_clamp_clevis.stl) | 1 | 12.0 × 17.0 × 10.0 |
| [24 mm servo link](stl/12_servo_connecting_link_24mm.stl) | 1 | 6.0 × 30.0 × 2.6 |
| [Base foot](stl/13_glue_on_base_foot.stl) | 4 | 10.0 × 10.0 × 4.0 |

## Use the new matching mechanism

Do not mix the earlier head, stem, lid or pot with this set, or resize these STLs in the slicer.

- The six head links are now **19.5 mm between centres**. The base servo link remains 24 mm.
- Form the head ring from **1.0 mm brass wire**, with **8.25 mm between opposite wire centrelines**. The crossbar connects opposite vertices. Slide the links onto the ring before closing it.
- The straight pushrod is **1.5 mm brass rod**, approximately **115.7 mm from its lower tip to the crossbar centreline**. Trial-fit before trimming.
- Use three **M2 × 8 mm** bolts and M2 nuts to attach the head. The old 12 mm head bolts are too long for this revision.
- Use 1.5 mm hinge pins with nominal 1.8 mm bores. The fixed-pivot reference pins are 9.75 mm long and fork pins 5.25 mm; allow enough exposed length for your chosen retainers.
- SG90 horn pivot radius remains 8 mm. Rod travel is now **7.49 mm** and the horn sweep is about **55.83°**. Recalibrate endpoints; do not reuse the previous values.

## Printing

Import in **millimetres at 100% scale** and choose the actual printer/nozzle/material profile. No printer-specific G-code is included. All individual parts fit within 180 × 180 × 180 mm before adding brim/support.

For PLA and a 0.4 mm nozzle, a starting point is 0.16 mm layers for small parts, 0.20 mm for the base, 3 walls, 4 top/bottom layers and 20–30% infill. These are untested starting settings. The scaled petal shell is about 0.9 mm thick radially, and head-link eye walls are about 0.8 mm; inspect the actual extrusion paths for missing thin sections.

Petals are exported on their sides and **need supports** beneath the curved shell and root. Print the stem upright with an 8–10 mm brim, keeping supports out of its internal guide bores. Check cone windows, nut pockets, hinge overhangs and cable-tie tunnels; use only removable support. Print links flat with bores vertical, the cup open-side up and the lid underside-down.

Print one inner petal, one outer petal, the hub, one 19.5 mm link and the servo cradle first. Check pin and servo fit before printing every copy. Move the assembled mechanism by hand before attaching motor power.

## Checks

All 12 exported STLs passed the [mesh audit](print-audit.json). The assembly passed 61 sampled collision checks with approximately 0.71 mm sampled link-to-connector clearance. [Motion and size results](validation.json). Physical fit, strength and motor performance remain untested.

This is a reconstruction inspired by the visible Jiří Praus flower mechanism, with an independently designed SG90 base; it is not the creator's original CAD.

