# PZT Element Preparation 

The PZT elements each have slightly different widths and thicknesses, due to deviations from the nominal values given on the datasheet (tolerances provided by the manufacturer for these PZT elements were \(\pm\) 130 \(\mu m\) for width and \(\pm\) 25 \(\mu m\) for thickness, detailed in: [`Piezoelectric Element Tolerances - APC International.pdf`](https://github.com/morganjroberts/open-UST/blob/main/hardware-distribution/technical-datasheets/Piezoelectric%20Element%20Tolerances%20-%20APC%20International.pdf)).

It is useful to measure these dimensions:

* The element widths are needed for calibrating the slot widths in the matching layer deposition mould, and the PZT alignment mould.
* If the unmatched and matched PZT element thicknesses are measured, these can be used to estimate the matching layer thicknesses (this data can be useful for quality control and when interpretting inter-element variations in acoustic performance).

## Load the PZT Element Tray

To store and keep track of the PZT elements, a gridded tray has been designed. This is accompanied by spreadsheet [`pzt-element-dimensions-defects.xlsx`](https://github.com/morganjroberts/open-UST/blob/main/hardware-distribution/pzt-element-dimensions-defects.xlsx), where the data rows and columns correspond to the physical row and column locations on the PZT element tray. Each PZT element should be assigned a PZT ID matching its row/column location in the storage tray e.g. 'A/3'.

![PZT-element-tray](img/pzt-element-preparation/PZT-element-tray.jpg)

1. Manufacture the PZT storage tray (further details [here](custom-tooling-manufacture.md)).
1. Load the tray with PZT elements, using plastic tweezers.
1. Use M3 x 12 mm screws to secure the lid to the tray for storage.

## Dress the PZT Electrode Edges

* During manufacture the individual PZT bars are cut from a large slab. Sometimes the silver electrodes are not cut neatly to the edge of the PZT.
* The excess PZT electrode material can fold over onto itself during shipping and handling.
* The excess electrode can affect the thickness measurement of the PZT elements and can prevent the PZT elements from seating properly on the bottom face of the slots in the PVA mould during matching layer deposition.
* To fix this, the electrode edges should be "dressed" by scraping away the excess electrode material.

For each PZT element:  

1. Remove the PZT element from the tray using tweezers.
1. Hold the PZT element on a flat clean surface, under a microscope, with the electrode facing upwards.
1. Use a scalpel blade to gently chamfer the edges of the electrodes. Do not apply excessive downwards pressure with the scalpel. Do not touch the face of the electrode with the scalpel.

![dressing-electrodes](img/pzt-element-preparation/dressing-electrodes.png)

## Meaure the PZT Element Dimensions

1. Setup a micrometer securely in a clamp on a workbench.
1. Clean the micrometer anvils using a foam swab and isopropyl alcohol.
1. If using a digital micrometer, calibrate/tare it to 0.
1. Remove a PZT element from the storage tray with tweezers and clean using a foam swab and isopropyl alcohol.
1. Align the PZT element so that the electroded faces are parallel with the micrometer anvils.
1. Turn the ratcheting (rear-most) micrometer screw until it clicks.
1. Record the PZT element thickness.
1. Rotate the element so that the non-electroded faces are parallel with the micrometer anvils.
1. Record the PZT element width.
1. Gently drop the PZT element into the correct location in the PZT element tray, being careful not to scrape the PZT element against the hole wall.
1. Repeat for all PZT elements.

**Note:** Re-clean the micrometer anvils using a foam swab and isopropyl alcohol every 10 PZT elements.

![pzt-thickness-measure](img/pzt-element-preparation/pzt-thickness-measure.png)

## Example Data

Width and thickness distributions were measured from the pool of PZT elements (N = 288) used for this project, using the procedure detailed above. Excess electrode folding was found to produce a systematic error in thickness measurement. A mean decrease of 22 \( \mu m \) was measured before and after dressing the electrode edges. The difference in standard deviation was negligible after dressing. In this case, the mean values for thickness and width match the nominal value provided by the manufacturer.

| Dimension                  | Mean [\( \mu m \)] | Standard Deviation [\( \mu m \)] |
| ---                        |    ----            |          ---                     |
| Thickness (Pre-dressing)   | 1021               | 8.2                              |
| Thickness (Post-dressing)  | 999                | 8.4                              |
| Width                      | 1000               | 20.4                             |

![pzt-element-dimensions](img/pzt-element-preparation/pzt-element-dimensions.png)

## Element Assignment

Make a list of PZT element IDs, ordered by their width. Matching layer deposition and PZT element alignment will be performed in batches. Within each batch, it is important that the PZT element widths are approximately equal.