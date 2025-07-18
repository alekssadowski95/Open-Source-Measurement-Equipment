> [!NOTE]
> **Suppliers wanted** <br>
> Become a supplier, by adding your info to the BOM and uploading a CAD file of your component to CAD/Supplier as a STEP file.

# Open-Source Measurement Equipment
Open-source framework for designing and manufacturing measurement equipment devices:
- Digital Oscilloscopes
- Waveform Generators
- Spectrum Analyzers
- RF Generators
- Vector Network Analyzers
- RF Switch Systems
- Digital Multimeters
- DC Electronic Loads
- Power Supplies

![librevna-enclosure.jpeg](librevna-enclosure.jpeg)
*Figure 1: Enclosure for the LibreVNA PCB*


## Formfactors
- 10 inch touchscreen
- 7 inch touchscreen
- 5 inch touchscreen

![measurement-equipment-formfactors.jpeg](measurement-equipment-formfactors.jpeg)
*Figure 2: Different measurement equipment formfactors with screen sizes of 10, 7 and 5 inches*


## Front panel design types
- Screen
- Analog controls
- Connectors

![measurement-equipment-front-panel-layouts.jpeg](measurement-equipment-front-panel-layouts.jpeg)
*Figure 3: Four Different front panel design types based on the layout of the screen, analog controls and connectors.*


## Bill of materials (10 inch touchscreen, type I, mechanical)
*Table 1: Bill of materials for a device with a 10 inch touchscreen and type I front panel layout including the price and supplier for the components.*
| Item no. | Description                                                | Count | Price | Supplier |
|----------|------------------------------------------------------------|-------|-------|----------|
| 1  | Measurement equipment PCB                                  |   1   |       |          |
| 2  | Steel enclosure frame                                      |   1   |       |          |
| 3  | Raspberry PI 5                                             |   1   |       |          |
| 4  | SD card                                                    |   1   |       |          |
| 5  | PSU for Raspberry PI 5                                     |   1   |       |          |
| 6  | USB-C cable                                                |   1   |       |          |
| 7  | Fan for steel enclosure                                    |   1   |       |          |
| 8  | PSU for fan                                                |   1   |       |          |
| 9  | Plastic or rubber feet + screws for steel enclosure        |   4   |       |          |
| 10 | 3D-printed plastic front panel                             |   1   |       |          |
| 11 | Brand and model sticker                                    |   1   |       |          |
| 12 | Brass threaded inserts (?x)                                |       |       |          |
| 13 | 10 inch touch screen with HDMI                             |   1   |       |          |
| 14 | Touch screen mounting screws                               |   4   |       |          |
| 15 | Touch screen PSU                                           |   1   |       |          |
| 16 | Micro-HDMI to HDMI cable (correct?)                        |   1   |       |          |
| 17 | On button                                                  |   1   |       |          |
| 18 | On/off switch                                              |   1   |       |          |
| 19 | Mains connector                                            |   1   |       |          |
| 20 | Some way to connect all devices to mains                   |   1   |       |          |
| 21 | Handle                                                     |   1   |       |          |
| 22 | Handle mechanism                                           |   1   |       |          |


## Design reference
For reference on enclosure design.
- Rigol DHO800: https://www.youtube.com/watch?v=KQF4UzLPpr0
- Rohde & Schwarz HMO1202: https://www.youtube.com/watch?v=q_FBwu2K7j0
- Tektronix 2 Series Oscilloscope: https://www.youtube.com/watch?v=R2fw2g6WFbg
- Rohde & Schwarz MXO4: https://www.youtube.com/watch?v=BTuXbY_nBOM
- Tektronix MDO3000: https://www.youtube.com/watch?v=VFX47ZGOn_o
- Siglent SVA1015X VNA: https://www.youtube.com/watch?v=HxBcQDooAYs

-> A solution for some way to connect all devices to mains needs to be found<br>
-> A patent search for a handle mechanism has to be done or a mechanism from a device, that is at least 20 years old used.

## Patent search for handle mechanism
Patent search for handle mechanism on Espacenet (https://worldwide.espacenet.com/), that is over 20 years old.

*Table 2: Patent search queries on espacenet.com wit the number of results*
| Query                                                                                   | No. of results |
|-----------------------------------------------------------------------------------------|----------------|
| pd <= "2005-01-01"                                                                      | 33 676 350     |
| ia = "tektronix" AND pd <= "2005-01-01"                                                 | 3 721          |
| ia = "tektronix" AND nftxt = "handle" AND pd <= "2005-01-01"                            | 251            |
| ia = "tektronix" AND nftxt = "handle" AND nftxt = "mechanism" AND pd <= "2005-01-01"    | 78             |


*Table 3: Relevant patents from patent search*
| Document no.                                                                                                                    | Title                                                                   |
|---------------------------------------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------|
| [US6140812A](https://worldwide.espacenet.com/patent/search/family/022275362/publication/US6000097A?q=pn%3DUS6000097A)           | Electronic instrument with multiple position spring detented handle     |



## Device 1: 10 inch touchscreen, type I , LibreVNA
LibreVNA (PCB, GUI) (https://github.com/jankae/LibreVNA)

1. Find suppliers for components
2. Get CAD files (*.STEP) for supplied bought components
3. Create assembly in FreeCAD, import all supplier components and arrange them
4. Design all remaining components in FreeCAD
5. Get supplier parts, manufacture custom parts and assemble device
6. Showcase project in nanoPLM (https://github.com/alekssadowski95/nanoPLM)
