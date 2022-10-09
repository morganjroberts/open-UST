# Rigid Coating

## Seal Cable-Transducer Entry Point

1. Mount the transducer in the custom vertical clamp (further details [here](custom-tooling-manufacture.md)), taking care not to damage the PZT elements during handling.
1. Hold the cable in place vertically.
1. Clean the cable entry point and surrounding copper foil and braid using isopropyl alcohol and a foam swab.
1. Allow the solvent to evaporate.
1. Dispense equal parts (by volume) of Loctite EA9455 toughened epoxy onto a sacrificial piece of masking tape (~2 ml total).
1. Mix thoroughly for 1 minute using a small plastic rod, making sure all material is fully incorporated.
1. Use a foam swab to apply the epoxy to the cable entry point, forming a smooth fillet around the circumference. Make sure the joint completely covers the seam between the copper foil and the exposed housing region, to prevent leakage.

![seal-cable-entry-point](img/rigid-coating/seal-cable-entry-point.png)

## Prepare Coating Moulds

1. 3D-print the coating mould parts (orientation and slicer settings detailed in [3D-print-spec.pdf](https://github.com/morganjroberts/open-UST/blob/main/hardware-distribution/3D-print-spec.pdf)).
1. Allow the parts to cool for 1 hour.
1. If the parts are not being used immediately, store them in a sealed container to prevent dimensional changes due to humdity.
1. Cleanup nozzle stringing using a scalpel, and use an air duster to blow debris out of the parts.
1. Install M3 threaded inserts into the rigid coating split mould, using a soldering iron set to 275 °C. Make sure the top of the insert sits below the surface of the part to allow full contact between mating faces during assembly.
- Part A has x2 inserts
- Part B has x8 inserts
1. Use a scalpel to flatten any PVA squeezeout around the threaded inserts.
1. Use a paper towel to apply a layer of vaseline petroleum jelly to the threads of the M3 x 6 mm socket head bolts.

![prepare-coating-moulds](img/rigid-coating/prepare-coating-moulds.png)

## Assemble Coating Moulds

1. Degrease the sides of the transducer module using a paper towel soaked in isopropyl alcohol. Do not degrease the front face yet.
1. Use a fine paint brush to apply a bead of washable PVA glue onto the mating faces of each half of the rigid coating mould. 
1. Place the two halves of the mould either side of the transducer cable.
1. Install 6 M3 x 20 mm socket head screws through part A, into the threads in part B, to clamp the split mould together.
1. Use a foam swab to remove the PVA squeezeout inside the mould cavity, so that the internal mould seam is smooth.
1. Allow the PVA adhesive to dry for 1 hour.
1. Remove the M3 x 20 mm clamping screws from the mould.
1. Pull the transducer module through the mould so that the mounting nuts are aligned with the corresponding holes in part A.
1. Install the greased M3 x 6 mm socket screws to attach the transducer module to the mould. Tighten the screws so that there is no epoxy leakage during coating.
1. Dispense silicone sealant onto a sacrificial paper towel.
1. Use a foam swab to plug all of the holes in the coating mould with silicone sealant.
1. Use a gloved finger to seal the cable entry point to the mould with silicone sealant. A thick layer is needed since the PVC-silicone bond is weak. A thin coat could easily peel away when the transducer is handled.
1. Allow the silicone sealant to cure for 4 hours.

![assemble-coating-moulds](img/rigid-coating/assemble-coating-moulds.png)

## Fix Coating Mould to Strongplate

1. Manufacture the coating mould strongplate (further details [here](custom-tooling-manufacture.md)).
1. Install M3 screws through the strongplate and into the coating mould-transducer assembly (part A should be facing the strongplate).
1. Tighten the screws so that part A is pulled flat against the strongplate.
1. Install the acoustic coating mould using M3 x 8 mm screws.
1. Use a safety blade to test the transducer-mould alignment. The PCB should be level with the top surface of the acoustic coating mould.
1. Remove the acoustic coating mould.
1. If the PCB was too low, reduce the height of the acoustic coating mould by lapping it on a sheet of P180 grit abrasive paper.

![assemble-coating-mould-strongplate](img/rigid-coating/assemble-coating-mould-strongplate.png)

## Cast Rigid Coating

- **Note:** the working time of Glass Cast 10 is \(\geq \) 45 minutes, which is long enough that it this is not a limiting factor for the number of transducer modules that can be coated in one batch.
- **Note:** Be careful not to touch the front face of the transducer with the epoxy. If this happens, remove it immediately and rinse thoroughly with isopropyl alcohol.
- **Note:** The pigment is for cosmetic purposes only. Omitting it will not affect the curing properties of the epoxy.

Cast the coating using the following procedure:

1. Use an air duster to remove debris from the front face of the transducer module.
1. Use a foam swab and isopropyl alcohol to degrease the front face of the transducer module.
1. Test the fit of the 15ga blunt needle in the coating cavity.
1. If the needle is slightly too large, compress it in a vice until it fits.
1. Tightly push the needle luer-slip fitting onto the 60 ml syringe barrel and remove the plunger.
1. Calculate the required mass of resin, hardener and pigment. For four transducer modules, the required volume is 60 ml, and the required quantities are:

| Component | Mass [g] |
|-----------|----------|
|Resin |44.68|
|Hardener |20.11|
|Pigment |6.48|

1. Place a clean mixing pot on a digital balance (resolution 0.1 g or better), and tare it.
1. Dispense the required mass of resin.
1. Tare the balance.
1. Dispense the required mass of hardener.
1. Tare the balance.
1. Dispense the required mass of pigment.
1. Use a plastic rod to mix the components together for 5 minutes. Frequently scrape down the walls and bottom of the pot to make sure that all of the material is fully incorporated.
1. Pour the mixture into the syringe barrel.
1. Holding the syringe horiztonally, push the plunger into the syringe barrel until it forms a seal, but no further.
1. Gently rotate the syringe so that it is vertical, with the needle facing up, and allow the mixture to settle and for the air to rise to the top.
1. Slowly push the plunger to expell all of the air from the syringe.
1. Place the needle into the coating mould cavity, as far down as it will go (it may be necessary to wiggle the needle if the fit is tight).
1. Gently push the syringe plunger to dispense the epoxy into the mould.
1. Once the epoxy has reached the top of the mould, gently remove the needle from the mould.
1. Wait for 10 minutes to check that the epoxy is not internally into the transducer module, indicated by the level going down without visible external leaking (see note below).
1. Place the acoustic coating mould over the exposed transducer module.
1. Install 4 M3 x 8 mm screws to secure the acoustic coating mould to the rigid coating mould.
1. Allow to cure for 24 hours.

**Note:** If the epoxy is leaking internally, it will leak into the cable, making the cable rigid when the epoxy cures, which should be avoided. To stop a leak, use the needle and a new syringe to suck as much epoxy as possible out of the mould, wait for the epoxy to cure (this will seal the leak) and start the coating process again with a new batch of epoxy.

![cast-rigid-coating](img/rigid-coating/cast-rigid-coating.png)
