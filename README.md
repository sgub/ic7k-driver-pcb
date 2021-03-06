# Improved IC-7000 HF/VHF/UHF Transceiver driver stage PCB

## Features:
* Reduce pinheader spacing from 1.5mm to 1.27mm, for better availability of parts and easier mating with the PA board.
* Added resistor R103 in series with the gate of the MOSFET, to suppress self oscillication on certain conditions which could burn-off the driver module.

## BOM:
* Q504: ST Microelectronics PD55015-E 550MHz/15W MOSFET, PowerSO-10 Package, formed lead.
* R103: Choose a value by experiment from 1ohm (moderate damping) to 10ohm (~50% reduced final output power on UHF, but much safer), size 0805
* R102: 100ohm/1W, Axial_DIN0309_L9.0mm_D3.2mm_P15.24mm. Size is critical due to limited installation space.
* J107,J104,J103,J102,J101: PinHeader_1x04_P1.27mm_Vertical, 11mm total height.
* C102: 39pF/100V, Size 1206.
* C101: 10nF/50V, size 0805.

## Build notes:
* Prefered board material is FR4 double layer, 1.6mm thick.
* Apply enough solder between the underside of the MOSFET and the heatsink for effective heat conducting, avoid space, soldering/heating with proper tool. Refer STMicroelectronics AN1294 Application note for temperature limit and technique recommendation.
