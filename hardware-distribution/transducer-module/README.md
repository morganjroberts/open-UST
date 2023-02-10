# Transducer Module 

<p align="center">
  <img src="https://github.com/morganjroberts/open-UST/blob/main/docs/img/cad-images.png" width="100%">
</p>

The transducer module source files are found within `transducer-module.f3d`. The CAD file is split into the following components:

| Component | Type | Description |
|---|---|---|
| PZT Elements | Transducer part | PZT elements with matching layers.|
| PCB | Transducer part | Interconnect PCB used to interface cable with PZT elements. |
| Backing Layer | Transducer part | Cast behind the PZT elements to provide damping. |
| SMT Header | Transducer part | Surface mount header strip soldered to interconnect PCB to mate with cable IDC connector. |
| IDC connector | Transducer part | Crimped onto ribbon cable, mates with SMT header. |
| Housing | Transducer part | 3D-printed backbone of the transducer module. PCB and backing layers are bonded to this. Cable fixed to this. |
| Ribbon Cable | Transducer part | Round bundled ribbon cable in overall sheath. IDC connector is crimped to this. |
| Cover | Transducer part | Completes the housing after the cable is fixed in place. |
| PZT Alignment Mould | Sacrifical custom tooling | Aligns the PZT elements during manufacture, gets dissolved in water to remove it. |
| Clamp | Re-usable custom tooling | Clamps the housing to the base plate during backing layer casting. |
| Base Plate | Re-usable custom tooling | Holds the PCB, housing, and PZT alignment mould together during manufacture. |
| Mounting nuts | Transducer part | Glued into the housing, used to fix the transducer module to the array mounting plate. |
| Coatings | Transducer part | Epoxy and polyurethane coatings to protect the transducer modules. |
| Coating Moulds | Sacrificial custom tooling | Used for casting the coating layers around the transducer module. |
| Inclined Jig | Re-usable custom tooling | Used to hold the base plate at a 45 degree angle during application of conductive epoxy to the PZT electrodes. |
| Rigid Aperture Support | Additional part | Used to mount the transducer modules into a 2D ring array configuration. |
| Testing Mount | Additional part | Used to hold a single transducer module vertically during cable entry-point sealing, or electrical input impedance measurement. |
| Shielding Templates | Re-usable custom tooling | 2D templates to mark out the copper foil pattern nets electromagnetic shielding. |
| Coating Strong Plate | Re-usable custom tooling | Used to hold the coating moulds vertically and flat, to eliminate warping during casting. |
| Single Module Tank Mount | Additional part | Used to mount a single transducer module to an optical post for immersion in water e.g. for hydrophone scanning. |
| Storage Box | Additional part | Used to hold 8 transducer modules to protect their front faces from damage during storage. |