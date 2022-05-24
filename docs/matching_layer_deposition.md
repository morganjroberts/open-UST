# Matching Layer Deposition

## Dress the PZT electrode edges

* The PZT electrode edges can become damaged  during their manufacture and shipping.
* In some cases, they can delaminate from the PZT and fold over onto themselves.
* This can affect the thickness measurement of the PZT elements and can prevent the PZT elements from seating properly on the bottom face of the slots in the PVA mould during matching layer deposition.
* To fix this, the edges should be "dressed" by scraping away the raised electrode.

1. Perform this work underneath a microscope.
2. Hold the PZT element using tweezers (ideally plastic, to avoid scratching the electrode).
3. Use a scalpel blade (Swann-Morton No.11) to gently chamfer the edges of the electrodes.

**Notes:** Do not apply excessive downwards pressure with the scalpel. Do not touch the face of the electrode with the scalpel.

`placeholder for video`

## PZT Dimension Capture
It is helpful to measure the dimensions of the PZT elements before depositing the matching layers:

* The actual PZT dimensions will differ from the nominal values given on the datasheet (tolerances provided by the manufacturer for these PZT elements were \(\pm\) 130 \(\mu m\) for width and \(\pm\) 25 \(\mu m\) for thickness, detailed in: [`Piezoelectric Element Tolerances - APC International.pdf`](https://github.com/morganjroberts/open-UST/blob/main/hardware-distribution/technical-datasheets/Piezoelectric%20Element%20Tolerances%20-%20APC%20International.pdf))
* Knowing the distribution of element widths and thicknesses is useful for calibrating the slot widths and depths in the matching layer deposition mould. 
* If the unmatched and matched PZT element thicknesses are measured, these can be used to estimate the matching layer thicknesses. This data can be useful to interpret inter-element variation in acoustic performance.

### Manufacture the PZT Element Tray

To keep track of the PZT elements, a gridded tray has been designed.

![doctor_blade_coater_print_orientation](../img/matching-layer-deposition/pzt-dimension-capture/PZT Element Tray.jpg)

**Note:** The default stl file is [`PZT Element Tray 16x17 10 mm length.stl`](https://github.com/morganjroberts/open-UST/blob/main/hardware-distribution/pzt-element-tray/PZT%20Element%20Tray%2016x17%2010%20mm%20length.stl), which is a 16 \(\times\) 17 grid, supporting 272 PZT bars of dimensions 1 mm \(\times\) 1 mm \(\times\) 10 mm. To design a tray for more elements, or for elements with different dimensions, open the [`pzt-element-tray.f3d`](https://github.com/morganjroberts/open-UST/blob/main/hardware-distribution/pzt-element-tray/pzt-element-tray.f3d) CAD file in Fusion 360 and edit the `Nrows, Ncolumns, hole_diameter, pzt_element_length` parameters in the `Solid > Modify > Change Parameters` menu.

1. Print the stl file with these settings:
    * Low infill < 20% (non-structural)
    * Coarse layer height 0.2 mm
    * No support required
    * Preview the part and make sure the holes are empty

2. Install the threaded inserts into the holes using a soldering iron set to 275\(^{\circ}\)C (adjust as necessary for non-PLA filaments),
3. Manufacture a perspex lid with 4 mm clearance holes. If using the default stl file, the [`PZT Element Tray Drawing.pdf`](https://github.com/morganjroberts/open-UST/blob/main/hardware-distribution/pzt-element-tray/PZT%20Element%20Tray%20Drawing.pdf) drawing can be printed out at 100% size to help mark out the hole pattern.
4. Label the rows with numbers and columns with letters using a permenant marker.
5. Use M3 screws to secure the lid to the tray (part ID XXX in BOM).

BATCHES

### Meaure the PZT element dimensions

![doctor_blade_coater_print_orientation](../img/matching-layer-deposition/pzt-dimension-capture/Micrometer Measurement.jpg)

The PZT element dimensions should be recorded in spreadsheet XXX, where the data rows and columns correspond to the physical rows and column locations on the PZT element tray. From now on, the element should be identified by its row/column location e.g. 'A/3'.

1. Setup a micrometer (this project used Mituyo XXX) securely in a clamp on a workbench.
2. Clean the micrometer anvils using a foam swab (part ID XXX in BOM) and acetone.
3. If using a digital micrometer, calibrate/tare it to 0.
4. For each PZT element:
    * Carefully handle the PZT element using tweezers (plastic if possible)
    * Clean the PZT element using a foam swab and acetone.
    * Align the PZT element so that the electroded faces are parallel with the micrometer anvils.
    * Turn the ratcheting (rear-most) micrometer screw until it clicks.
    * Record the thickness measurement.
    * Rotate the element so that the non-electroded faces are parallel with the micrometer anvils.
    * Record the PZT element width.
    * Gently drop the PZT element into the correct location in the PZT element tray, being careful not to scrape the PZT element against the hole wall.

**Note:** Re-clean the micrometer anvils using a foam swab and acetone every 10 PZT elements.

`placeholder for video`

## Manufacture Doctor Blade Coater
The doctor blade coater uses a 3D-printed blade holder to hold a safety blade at the correct angle. It is used during the deposition of the tungsten-epoxy quarter-wavelength-matching-layers to scrape the compound over the PZT elements.
![doctor_blade_coater_print_orientation](../img/matching-layer-deposition/doctor-blade-coater/doctor_coater_dissassembled.jpg)


### Set the Rail Height and Other Parameters
To set the blade angle, the correct thickness of the QWML-deposition mould must be specified.
(This step is only required if a non-standard PZT thickness is being used: If the nominal PZT thickness is approximately 1 mm, skip this step).

* Open the `QWML-deposition-mould.f3d` CAD file in Fusion 360,
* Record the `calculatedPartHeight` value from the `Solid > Modify > Change Parameters` menu,
* Open the `doctor-blade-coater.f3d` CAD file in Fusion 360,
* In the `Solid > Modify > Change Parameters` menu, set the `bladeHeight` parameter to the same value as `calculatedPartHeight`.
* Export the blade-holder and support-arm as .stl files.

**Notes:**

* This doctor blade coater is designed for a specific safety blade (RS PRO 546-758). If a different blade is used, the blade dimensions should be updated in the 'Change Parameters' menu.
* The standard `bladeAngle` parameter used is 45 degrees. Preliminary testing showed that steeper blade angles produce a rougher surface finish, and that shallower blade angles require excessive downwards pressure, which can lead to blade-flexing and non-uniform matching layer thickness.

### 3D-printing

* Load `blade-holder.stl` and `support-arm.stl` into the Cura slicer software.
* Use the following print orientation, to make sure the blade-holding features are flat. Use the 'Select face to align to the build plate' function.

![doctor_blade_coater_print_orientation](../img/matching-layer-deposition/doctor-blade-coater/doctor_blade_print_orientation.png)

Recomended Settings:

* Use 100% infill to make the blade-holder as stiff as possible, so that the blade can be clamped flat,
* PVA support required for `blade-holder.stl` but not for `support-arm.stl`.
* 0.2 mm layer thickness,
* Enable top support interface.

### Process the Blade-holder

* A smooth flat surface is required to clamp the blade without flexing,
* Use a scalpel to remove bumps created by the 3D-printer nozzle. 

<div align="center">    
    <iframe width="560" height="315" src="https://www.youtube.com/embed/OjL9OB76LAg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
<br/>


### Install Threaded Inserts

* Use a soldering iron set to 275 degC,
* Place the M3 threaded insert [part ID 0] on to the soldering iron tip,
* Place the insert into the hole and push gently,
* As the plastic melts, push the insert into the hole, making sure that the insert is properly aligned.
* Keeping pushing until the insert sits below the surface,
* Gently twist the solering iron to remove it.
* Once all the inserts are installed, remove the raised edge around the insert by scraping with a scalpel.

### Install the Safety Blade

* Degrease the blade using Isopropyl Alcohol and a paper towel.
* Attach the support-arm to the blade-holder using x2 of M3 x 12 mm screws [part ID 1].
* Pre-install x4 of M3 x 6 mm screws [part ID 2] into the blade holder, leaving space for the blade. Use washers [part ID 3] for the two outermost screws near the blade tips.
* Slide the safety blade underneath the heads of the screws. Make sure the blade is fully seated against the registering features.
* Gently tighten the screws, using the lowest tension required to grip the blade. Overtightening will lead to blade flex.
* Look along the blade to check its straightness. If there is a visible bend, check that the screws are not overtightened, and that the clamping surfaces are flat and clean.

## Batching

## Slot width calibration
### Process width and thickness data
* Sort PZT elements into ascending width order
* Decide thickess

## Print Matching Layer Deposition Mould

## Load PZT Elements into Deposition Mould

## Tungsten-Epoxy Composite Preparation
### Prepare Vacuum Mixing Bag
### Measure Components into Bag
### Remove Air and Seal Bag
### Mix Components

## Tungsten-Epoxy Doctor Blade Coating

### Print Doctor blade coater

## Dissolve PVA Mould

## Trim Matching Layers









