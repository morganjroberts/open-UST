# PZT Element Alignment
Slot width affects orientation in lateral plane
elevation plane easier 


## Description

## Manufacture Steps
### Probe assignment by PZT element width
Transducer modules should contain PZT elements with similar widths, so that a constant slot width can be used.


### Calibrate Alignment Mould Slot Width
The slot width should be tuned for every transducer module. Slot width calibration should be performed immediately before printing the final alignmnet-mould for a given transducer module, because deviations in 3D-printer filament diameter can cause drift in 3D-printer linewidth over time.

The alignment mould slot width must be as close as possible to the width of the PZT elements. This is so that the PZT elements cannot rotate in their slots.

These other parameters must be controlled to minimise the gap between the PZT elements and the alignment mould, so that the PZT element location is well known:
- PCB offset
- slot corner radius
- slot length
- 

Tune the slot width:
- print `piece.stl`
- choose the two elements with the largest width
- insert the pzt elements into all of the slots. The element should seat easily into the slots without needing force, but it should not rotate in the slots.


### 3D-print Alignment Mould

1. Adjust the slot width in CAD and export the new stl file,
2. Print the stl file with the following orientation and settings:
`image`
3. Label the part, marking the first (1) and last (16) element positions,
4. Allow the part to cool for 1 hour,
5. If the part is not being used immediately, store it in a sealed container to prevent dimensional changes due to humdity,
6. Cleanup nozzle stringing using a scalpel,
7. Use an air duster to blow debris out of the slots.

### Clean and load PZT into alignment mould slots

1. Hold the alignment mould with the blind end of the slots on the left and the PCB recess on the right.
2. Identify the PZT element ID for the first position, and remove the PZT element from the PZT tray using tweezers,
2. Under a microscope, lightly abrade the surface of the rear electrode using a small piece of P2000 grit sandpaper held in a pair of forceps. Do not remove excessive material,
3. Clean all faces of the PZT element using isopropyl alcohol and a foam swab,
4. Place the element on a clean surface and allow the solvent to evaporate,
5. Using a fine brush, paint the bottom of the alignment mould slot with washable PVA adhesive. Apply a thin coat, avoiding the side walls (excess PVA could squeeze onto the rear electrode, preventing bonding to the backing layer),
6. Wash the brush in water,
6. Using plastic tweezers, slide the clean PZT element into the slot, with the matching layer facing down, and the exposed front electrode on the right hand side, above the PCB recess.
7. Apply gently pressure with the tweezers to fully seat the element onto the bottom of the slot. Make sure the element is pushed fully into the blind end of the slot.
8. Repeat this process for all elements in the transducer module.

### Apply PVA blocking layer

A PVA blocking layer is needed to prevent the backing layer composite from bonding to the exposed front electrode (this would later obstruct an electrical connection from the electrode to the PCB pad).

1. Under a microscope, apply a small drop of washable PVA adhesive to the end of the PZT element with a fine brush. Do not cover the rear electrode. Cover the gap between the alignment mould and the PZT element, where the matching layer has been removed to expose the front electrode.
2. Repeat this process for all elements in the transducer module.
2. Allow the adhesive to dry for 30 minutes
3. Inspect the blocking layers. If the PVA adhesive does not completely block the gap next to the exposed electrode, apply a second blocking layer coat.

Note: if PVA adhesive is accidentally applied to the rear electrode, do not use solvent or water to remove it. Liquids can dissolve the surrounding PVA alignment mould and deposit a thin layer of PVA onto the rear electrode, preventing a proper bond between the electrode and the backing layer composite. Instead, allow the PVA adheisve to dry, then remove it using a small piece of P2000 grit sandpaper held in a pair of forceps. Remove the debris with an air duster.

