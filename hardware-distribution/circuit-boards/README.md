# Printed Circuit Boards

## Manufacture Specifications:
- 2 layer
- Plated through hole
- 1.6 mm thickness FR4 (150 deg C)
- 1 oz (35 micrometer) Copper weight
- Immersion silver finish
- Solder resist

## Notes
- UK PCB fabrication house: [pcbtrain.co.uk/services/pcb-fabrication](https://www.pcbtrain.co.uk/services/pcb-fabrication)
- The source files were created in DesignSpark PCB: [rs-online.com/designspark/pcb-software](https://www.rs-online.com/designspark/pcb-software)
- The Gerber files have already been exported and are found in a subfolder for each PCB. 
- Gerber files can be viewed here: [pcbway.com/project/OnlineGerberViewer.html](https://www.pcbway.com/project/OnlineGerberViewer.html)
- For each PCB, package the Gerber files into a .zip folder and send to the pcb fabrication house.
- If you have modified the DesignSpark source files, you will need to re-generate the Gerber files: [pcbway.com/helpcenter/technical_support/How_to_generate_Gerber_files_from_DesignSpark.html](https://www.pcbway.com/helpcenter/technical_support/How_to_generate_Gerber_files_from_DesignSpark.html)

## Module Interconnect

- This PCB is located inside each transducer module.
- Interfaces the ribbon cable IDC connector with the individual PZT elements.

<p align="center">
  <img src="https://github.com/morganjroberts/open-UST/blob/main/docs/img/pcb-housing-assembly/module-interconnect.png" width="50%">
</p>

## Module Matching

- This PCB is located inside the plug backshell.
- Interfaces each ribbon cable IDC connector with the DL5-260PW6A breakout stack.
- Contains pads for single-inductor electrical impedance matching on every channel (unbalanced).
- A XX package 22 uH inductor is recommended.
- These pads should be filled with zero-ohm links if no matching is required.

<p align="center">
  <img src="https://github.com/morganjroberts/open-UST/blob/main/docs/img/plug-assembly/module-matching.png" width="50%">
</p>

## DL5-260PW6A Breakout

- These PCBs form a stack that act as a breakout for the DL5-260PW6A plug connector.
- Provides a separate signal-ground pair for every channel (the plug pins share 2 ground pins per 8 signal pins).

<p align="center">
  <img src="https://github.com/morganjroberts/open-UST/blob/main/docs/img/plug-assembly/DL5-260PW6A-breakout.png" width="100%">
</p>

