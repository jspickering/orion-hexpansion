# Orion Starspansion

This is an Orion starspansion (hexpansion) for the [EMF Tildagon badge](https://github.com/emfcamp/badge-2024-hardware)

The guide below shows you which parts you need to make one yourself, and how to assemble it.

## materials

### mandatory

* Transparent acrylic sheet (1-3mm thick) (we ordered ours from [Hobarts]](https://hobarts.com/products/clear-cast-perspex-acrylic?variant=43939414245613)
* Opaque acrylic sheet (1-3mm thick) (we ordered ours from [Hobarts]](https://hobarts.com/collections/galaxy-acrylic)
* Custom starspansion PCB (schematic: FILENAME; we ordered ours from [JLCPCB](https://jlcpcb.com/), see appendix for details)
* 2mm LEDs (we ordered ours from [Switch Electronics](https://www.switchelectronics.co.uk/products/cool-white-2mm-lighthouse-diffused-lens-led-750mcd))
* 2x 20R resistors (we ordered ours from [PiHut](https://thepihut.com/products/resistor-packs?variant=37986550513859))
* 5x 100R resistors (we ordered ours from [PiHut](https://thepihut.com/products/resistor-packs?variant=37986550579395))
* 4x 1,000R resistors (we ordered ours from [PiHut](https://thepihut.com/products/resistor-packs?variant=37986550710467))
* 3D printing filament (we ordered ours from [Filamentive](https://www.filamentive.com/product/light-wood-3d-printing-filament-1-75mm-500g/))
* 4 inserts (2mm diameter) (we ordered ours from: )
* 4 screws (2mm diameter) (we ordered ours from: )


### optional

* wood stain (if using wood-based printing material)

## tools

* soldering iron + solder
* 3D printer
* laser cutter

## processes

1. Laser cut the acrylic using the appropriate schematics. For the transparent sheet, you should use the [FILENAME](), and for the opaque sheet you should use the [FILENAME]().

1. 3D print the three separate components of the chassis, using the design files for the [outer section](), [middle](), and [base](). We used a [wood-based filament]() which we then sanded down and applied 3 coats of wood stain to. But you can use any filament you want.
1. Using a laser cutter, cut the acrylic sheets. The top one should be cut with the design file for the [top layer](), and the bottom one with the design file for the [second layer]().

We used a [transparent acrylic]() sheet for the top (1mm thick), and a [galaxy-style sheet]() for the second layer (3mm thick). You can play around with different kinds, such as a translucent top sheet for a more diffused look. As long as the two layers total 4mm thick, everything else should slot together without needing to change any other aspects of the design.

1. Solder the LEDs and resistors. Here's how the LEDs and resistors map on (see the PCB itself), to get the correct magnitude for each star:

| LED ref | Resistor ref | Resistor value |
| ------------- | ------------- | ------------- |
| D1 | R1 | 20R |
| D2 | R2 | 20R |
| D3 | R3 | 100R |
| D4 | R4 | 100R |
| D5 | R5 | 100R |
| D6 | R6 | 100R |
| D7 | R7 | 100R |
| D8 | R8 | 1,000R |
| D9 | R9 | 1,000R |
| D10 | R10 | 1,000R |
| D11 | R11| 1,000R |

When you first put the LEDs in, you should use the middle part of the 3D printed chassis to ensure they're in the correct position before soldering (each pointed part of the LED should be visible in the holes when looking at it top-down -- there are some screw holes to help you hold it together if needed. You may need to take it off and put it back on a few times as you go. Finish with it slotted into the PCB and LEDs.

1. Take the base chassis piece, and gently place one of the inserts into one of the four holes (from the outside in). Using the soldering iron, gently place the tip on the insert and, using the heat of the iron, VERY SLOWLY AND CAREFULLY apply pressure so that the insert moves in. Ensure that it sits flush with the chassis piece. Repeat for the other 3 holes.

1. You can now start assembling the hexpansion. Take the outer section chassis piece, and slot the top layer acrylic in, followed by the second layer acrylic, followed by the PCB and middle chassis piece (middle chassis piece on top), and then the base chassis piece. Take the 4 screws and secure the base piece to the middle piece (outside in), using the inserts to thread in the screws. Don't screw it too tightly.



# Appendix
## Ordering the PCB
(WIP)