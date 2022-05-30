# PZT Element Preparation

The PZT element population will have a distribution of different widths and thicknesses, and some will have defects. In this section, these characteristics are measured and recorded. This information is used to select which elements should be used for the transducer modules. 

The data can also be useful when interpretting inter-element variations in acoustic performance.

It is helpful to measure the dimensions of the PZT elements before depositing the matching layers:

* The actual PZT dimensions will differ from the nominal values given on the datasheet (tolerances provided by the manufacturer for these PZT elements were \(\pm\) 130 \(\mu m\) for width and \(\pm\) 25 \(\mu m\) for thickness, detailed in: [`Piezoelectric Element Tolerances - APC International.pdf`](https://github.com/morganjroberts/open-UST/blob/main/hardware-distribution/technical-datasheets/Piezoelectric%20Element%20Tolerances%20-%20APC%20International.pdf))
* Knowing the distribution of element widths and thicknesses is useful for calibrating the slot widths and depths in the matching layer deposition mould. 
* If the unmatched and matched PZT element thicknesses are measured, these can be used to estimate the matching layer thicknesses. 

## Manufacture and Load the PZT Element Tray

To store and keep track of the PZT elements, a gridded tray has been designed. This is accompanied by spreadsheet XXX, where the data rows and columns correspond to the physical rows and column locations on the PZT element tray. From now on, each PZT element should be identified by its row/column location e.g. 'A/3'.

![doctor_blade_coater_print_orientation](../img/pzt-element-preparation/PZT Element Tray.jpg)

**Note:** The default stl file is [`PZT Element Tray 16x17 10 mm length.stl`](https://github.com/morganjroberts/open-UST/blob/main/hardware-distribution/pzt-element-tray/PZT%20Element%20Tray%2016x17%2010%20mm%20length.stl), which is a 16 \(\times\) 17 grid, supporting 272 PZT bars of dimensions 1 mm \(\times\) 1 mm \(\times\) 10 mm. To design a tray for more elements, or for elements with different dimensions, open the [`pzt-element-tray.f3d`](https://github.com/morganjroberts/open-UST/blob/main/hardware-distribution/pzt-element-tray/pzt-element-tray.f3d) CAD file in Fusion 360 and edit the `Nrows, Ncolumns, hole_diameter, pzt_element_length` parameters in the `Solid > Modify > Change Parameters` menu.

1. Print the stl file with these settings:
    * Low infill < 20% (non-structural)
    * Coarse layer height 0.2 mm
    * No support required
    * Preview the part and make sure the holes are empty

2. Install the threaded inserts into the holes using a soldering iron set to 275\(^{\circ}\)C (adjust as necessary for non-PLA filaments),
3. Manufacture a perspex lid with 4 mm clearance holes. If using the default stl file, the [`PZT Element Tray Drawing.pdf`](https://github.com/morganjroberts/open-UST/blob/main/hardware-distribution/pzt-element-tray/PZT%20Element%20Tray%20Drawing.pdf) drawing can be printed out at 100% size to help mark out the hole pattern.
4. Label the rows with numbers and columns with letters using a permenant marker.
5. Load the tray with PZT elements.
6. Use M3 x 12 mm screws to secure the lid to the tray during storage (part ID XXX in BOM).

## Dress the PZT Electrode Edges, Assess Defects

* During manufacture the individual PZT bars are cut from a large slab. Sometimes the silver electrodes are not cut neatly to the edge of the PZT.
* The excess PZT electrode material can fold over onto itself during shipping and handling.
* The excess electrode can affect the thickness measurement of the PZT elements and can prevent the PZT elements from seating properly on the bottom face of the slots in the PVA mould during matching layer deposition.
* To fix this, the electrode edges should be "dressed" by scraping away the excess electrode material.

![folded-electrode](../img/pzt-element-preparation/folded-electrode.svg)


**Note:** Perform this work underneath a microscope.

For each PZT element:  

1. Remove the PZT element from the tray using tweezers.
2. Hold the PZT element on a flat clean surface with the electrode facing upwards.
3. Use a scalpel blade (Swann-Morton No.11) to gently chamfer the edges of the electrodes. Do not apply excessive downwards pressure with the scalpel. Do not touch the face of the electrode with the scalpel.

`placeholder for video`

4. Assess the PZT element for any defects. Possible defects are chipping (C), electrode delamination (E), sliced electrode (S). Record these defects in spreadsheet XXX.

`placeholder for electrode damage example photo`

## Meaure the PZT Element Dimensions

![micrometer-measurement](../img/pzt-element-preparation/Micrometer Measurement.jpg)

1. Setup a micrometer (this project used Mituyo XXX) securely in a clamp on a workbench.
2. Clean the micrometer anvils using a foam swab (part ID XXX in BOM) and acetone.
3. If using a digital micrometer, calibrate/tare it to 0.
4. For each PZT element:
    * Carefully handle the PZT element using tweezers (plastic if possible)
    * Clean the PZT element using a foam swab and isopropyl alcohol.
    * Align the PZT element so that the electroded faces are parallel with the micrometer anvils.
    * Turn the ratcheting (rear-most) micrometer screw until it clicks.
    * Record the thickness measurement.
    * Rotate the element so that the non-electroded faces are parallel with the micrometer anvils.
    * Record the PZT element width.
    * Gently drop the PZT element into the correct location in the PZT element tray, being careful not to scrape the PZT element against the hole wall.

**Note:** Re-clean the micrometer anvils using a foam swab and acetone every 10 PZT elements.

`placeholder for video`

## Example Data

Width and thickness distributions were measured from the PZT elements (N = 288) used for this project, using the procedure detailed above. Excess electrode folding was found to produce a systematic error in thickness measurement. A mean decrease of 22 \( \mu m \) was measured before and after dressing the electrode edges. The difference in standard deviation was negligible after dressing.

| Dimension                  | Mean [\( \mu m \)] | Standard Deviation [\( \mu m \)] |
| ---                        |    ----            |          ---                     |
| Thickness (Pre-dressing)   | 1021               | 8.2                              |
| Thickness (Post-dressing)  | 999                | 8.4                              |
| Width                      | 1000               | 20.4                             |

![pzt-element-dimensions](../img/pzt-element-preparation/pzt-element-dimensions.svg)