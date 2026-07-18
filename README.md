# Orion Starspansion

![The full Orion Starspansion, plugged into the Tildagon 2024 badge](/images/orion_starspansion_1.jpg)

This is an Orion starspansion (hexpansion) for the [EMF Tildagon badge](https://github.com/emfcamp/badge-2024-hardware)

There's a [CAD model](/badge_model/Starspansion.f3z) if you want to see the complete hexpansion.

The guide below shows you which parts you need to make one yourself, and how to assemble it.

## Materials

### Core
These are all the materials you will need to create the hexpansion. We've linked to the exact products we used, but you can get them from whichever retailer you prefer.

* Transparent acrylic sheet (1-3mm thick) ([Hobarts](https://hobarts.com/products/clear-cast-perspex-acrylic?variant=43939414245613))
* Opaque acrylic sheet (1-3mm thick) ([Hobarts](https://hobarts.com/collections/galaxy-acrylic))
* Custom starspansion PCB ([JLCPCB](https://jlcpcb.com/), see [appendix](#appendix) for details on how to order them)
* 2mm LEDs ([Switch Electronics](https://www.switchelectronics.co.uk/products/cool-white-2mm-lighthouse-diffused-lens-led-750mcd))
* 2x 20R resistors ([PiHut](https://thepihut.com/products/resistor-packs?variant=37986550513859))
* 5x 100R resistors ([PiHut](https://thepihut.com/products/resistor-packs?variant=37986550579395))
* 4x 1,000R resistors ([PiHut](https://thepihut.com/products/resistor-packs?variant=37986550710467))
* 3D printing filament ([Filamentive](https://www.filamentive.com/product/light-wood-3d-printing-filament-1-75mm-500g/))
* 4x threaded brass inserts (M2 x 2 x 3.2) ([Amazon](https://www.amazon.co.uk/gp/aw/d/B0D41PW4GC?psc=1&ref=ppx_pop_mob_b_asin_title))
* 4x screws (M2 x 4) ([Amazon](https://www.amazon.co.uk/Premium-410-Piece-M2-Socket-Screw/dp/B0C1BMQK6T/ref=sr_1_10?dib=eyJ2IjoiMSJ9.ec2XkPjCTLphyCur4SjV1LYcDcoA4TuZfBRzJcCsZN54BXxc_tUUpMuCt5Guri9d9htPosCR-P9NZW7xD_XmA6NsZV3yxVAkDmSuLtaEWaK1z3YoWK5AJ6ooLgJkEJZBYKWCMzO-kyaV45lJbb8jfivTh59yqgS2k-A5ZM3MbI0ZODj77Q6jHUXQh-KLEhTx87yF_xTg8F0XrKIwPlFFHzyhw1RVGwhEqmd6leQLgxVd2MB7YCY5vhOgiUnW6GbrY0Hhkpiv1ALGMNfxzY1rKijh1VJ5ixGamhHxsz14tdk.U6UQpYHKPmatvGg9KSllMK7prQMRhpIz6KX31xTBUUw&dib_tag=se&keywords=m2%2Bscrews&qid=1784233113&sr=8-10&th=1))

![A desk displaying all the main parts for the hexpansion e.g. 3D printed chassis pieces, acrylics, and PCB](/images/parts.jpg)

### Optional
This is not necessary, but we used it when we created our version of the hexpansion.
* Wood stain (if using wood-based printing material)
* 2x M2 size screws to attach the hexpansion more securely to the badge

## Tools and equipment

* soldering iron + solder
* 3D printer
* laser cutter

## Processes

1) 3D print the three separate components of the chassis, using the design files for the [outer section](/printing_files/outer_section.stl), [middle](/printing_files/middle.stl), and [base](/printing_files/base.stl). We used a wood-based filament which we then sanded down and applied 3 coats of wood stain to. But you can use any filament you want.

2)  Using a laser cutter, cut the acrylic sheets. The top one should be cut with the design file for the [top layer without holes](/laser_cutting_files/acrylic_no_holes.dxf), and the bottom one with the design file for the [second layer with holes](/laser_cutting_files/acrylic_holes.dxf).

We used a transparent acrylic sheet for the top (1mm thick) just to add a bit of protection, and a galaxy-style sheet for the second layer (3mm thick) for a more space-themed look. You can play around with different kinds, such as a translucent top sheet for a more diffused look. As long as the two layers total 4mm thick, everything else should slot together without needing to change any other aspects of the design.

![Two acrylics -- a transparent top piece overlaid and offset from the galaxy second piece](/images/acrylics.jpg)

3) Solder the LEDs and resistors into the custom PCB. Here's how the LEDs and resistors map on (see the PCB itself), to get the correct magnitude for each star:

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

![The middle chassis -- a 3D printed piece with holes for the LEDs and resistors](/images/middle_chassis.jpg)

4) Take the base chassis piece, and gently place one of the brass inserts into one of the four holes (from the outside in). Using the soldering iron, gently place the tip on the insert and, using the heat of the iron, VERY SLOWLY AND CAREFULLY apply pressure so that the insert moves in. Ensure that it sits flush with the chassis piece. Repeat for the other 3 holes.

![The base chassis and middle chassis pieces, showing the brass inserts sitting flush with the 3D print](/images/base_chassis_inserts.jpg)

5) You can now start assembling the hexpansion. Take the outer section chassis piece, and slot the top layer acrylic in, followed by the second layer acrylic, followed by the PCB and middle chassis piece (middle chassis piece on top), and then the base chassis piece.

![A side view of the badge, showing the layering](/images/side_view.jpg)

Take the four screws and secure the base piece to the middle piece (outside in), using the inserts to thread in the screws. Don't screw it too tightly.

![A bottom view of the badge, showing the screws](/images/bottom_view.jpg)

And there it is. A complete Orion Starspansion hexpansion!

![A top view of the badge, showing the finished product](/images/top_view.jpg)

# Appendix
## Ordering the PCB
If you'd like to customise the PCB we've provided a [KiCad project](/PCB/starspansion_kicad/). If you just want to order the PCB, all you need is the [gerbers](/PCB/starspansion_kicad/gerbers.zip) .zip file. Head over to JLCPCB.com (or a PCB manufacturer of your choice) and select 'Order Now'. Drag and drop the gerbers .zip (or select 'Add gerber file') onto the upload area amd wait a few moments until the upload is complete and a visual representation of the PCB is displayed. The existing settings will be correct for the most part with two important exceptions:

* PCB Thickness: 1mm
* Surface Finish: ENIG

Feel free to choose the colour and number or copies as you'd like. Once you've chosen the settings, choose 'SAVE TO CART' and you can go ahead and head to your basket and place the order.