# Matching Layer Deposition

## Dimension Capture
It is helpful to meausure the dimensions of the PZT elements before depositing the matching layers. The actual PZT dimensions will differ from the nominal values given on the datasheet (tolerances provided by the manufacturer for these PZT elements were XXX for width and XXX for thickness, detailed in: [Piezoelectric Element Tolerances - APC International](../hardware-distribution/technical-datasheets/Piezoelectric Element Tolerances - APC International.pdf)).
Knowing the distribution of element widths is useful when calibrating the slot widths in the matching layer deposition mould. Knowing the distribution of element thicknesses is useful when defining the slot depth in the matching layer mould

Also, if the unmatched and matched PZT element thicknesses are measured, these can be used to estimate the matching layer thicknesses. This data can be useful to interpret inter-element variation in acoustic performance. Also, 

## PVA Deposition Mould Calibration
### Slot Width Calibration
The slot width must be calibrated to give a tight fit between the PZT elements and the matching layer deposition mould. This stops the PZT elements from rotating in their slots, which would make the matching layer thicker on one side of the PZT than the other.

* The standard width offsets are 0.08, 0.1, 0.12, 0.14mm
* The width offset depends on the layer height
* The width offset calibration part is a single 16-element row.
* It is evaluated by placing PZT elements into the slots and checking the tightness of fit manually and visually
* The ideal width offset is the tightest possible that 

Photos:
```
- [ ] Calibration Mould after printing on build plate
- [ ] Screenshots of CAD indicating the different offset groups
```
Video:
```
- [ ] testing element tightness with tweezers (Shot from above in booth) - re-print an old 0.03mmlayer file without copper foil for this.
```
### Slot Depth Calibration

Photos:
```
- [ ] Mould after printing on build plate
- [ ] Screenshots of checking the depth offset layers in the sliced model (Cura)
```
Video:
```
- [ ] Doctor blade coat tungsten-epoxy composite without PZT
```
## Print Doctor Blade Coater

* Calculate the height of the deposition-mould rail above the glass build plate: raft height + part height
* Input this into the Parametric CAD file for the doctor blade coater
* 3D print the parts 
* Assemble the parts

* Clamp should be 100% infill to make it as rigid as possible.
* Print orientation is important for doctor blade coater.

![doctor_blade_coater_print_orientation](../img/doctor blade coater/doctor_blade_print_orientation.png)

Photos:
```
- [ ] Dissassembled blade coater
- [ ] 3D print orientation of parts
```
Video:
```
- [ ] assemble doctor blade coater (threaded inserts, screwing with blade)
```

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

