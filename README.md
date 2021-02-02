# ic7k-driver-pcb
Improved driver stage PCB file for the IC-7000 HF/VHF/UHF all mode transceiver.

* Reduce pinheader spacing from 1.5mm to 1.27mm, for wider availability of parts and easier mating with the PA board.
* Added resistor R103 to suppress self oscillication on certain frequencies which could burn-off the Q504.

## BOM
* Q504: ST Microelectronics PD55015-E 550MHz/15W MOSFET, PowerSO-10 Package, formed lead.
* R103: Choose value between 1ohm and 1kOhm (~10% reduced output power, but safer), Size 0805
* R102: 100ohm/1W, Axial_DIN0309_L9.0mm_D3.2mm_P15.24mm. Size is critical due to limited installation space.
* J107,J104,J103,J102,J101: PinHeader_1x04_P1.27mm_Vertical, 14mm total height.
* C102: 39pF/100V, Size 1206
* C101: Choose value from 10nF (Original value) to 100nF(more feedback on higher frequency, safer).

