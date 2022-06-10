# Cable Preparation

A shielded round ribbon cable is used to connect each transducer module to the data acquisition system. The ends of each cable must be prepared by installing an insulation-displaement-contact (IDC) connector, and by terminating the copper braid,

## Cut Cable to Length

* Cut enough cable so that there is enough slack when the transducer modules are connected to the data acquisition system, and placed in the water tank.
* For this system, 2.3 m was the required length.
* Up to 122 mm of cable may need to be removed when the sheath length is adjusted (see below).
* To account for this the cables were cut oversized, to lengths of 2.5 m.

![cut-cable-to-length](img/cable-preparation/cut-cable-to-length.svg)

## Braid Preparation

The cable braid is made from groups of strands that are woven together. To prevent the braid from becoming untangled later, each group of strands should be terminated with solder.

1. Remove 25 mm of sheath using a scalpel.
    - **Note:** Use a fresh, sharp blade with light, shallow strokes.
    - **Note:** Take care not to cut the braid wires underneath the sheath. 
    - **Note:** Bend the cable to put tension on the sheath.
2. For each group of braid strands (see video below):
    - Use tweezers to pull the group of strands free from the braid,
    - Twist the end of the group,
    - Apply a small amount of solder to the end of the group of strands,
    - Bend the group of strands backwards.

![braid-preparation](img/cable-preparation/braid-preparation.svg)

` placeholder for video `

## Adjusting the Sheath Length

The length of ribbon cable between the end of the sheath and the IDC connector should be 36 mm \( \pm \) 5 mm. Deviations from this will it difficult to install the cable into the transducer module later.

The chosen cable has a continuous split/bond repeating pattern, where the split sections are 36 mm in length, and the bonded sections are 25 mm in length , detailed in [`3M-3659-3_34-way-screened-round-ribbon-cable_datasheet.pdf`](https://github.com/morganjroberts/open-UST/blob/main/hardware-distribution/technical-datasheets/3M-3659-3_34-way-screened-round-ribbon-cable_datasheet.pdf))

The end of the sheath should be aligned with the point where the ribbon cable changes from bonded to split (moving towards the end of the cable). This will provide approximately 36 mm of cable between the end of the sheath and the IDC connector. 

1. Use a scalpel to remove the foil, exposing the ribbon cable.
2. Mark the transition point where the ribbon cable changes from split to bonded (moving towards the end of the cable) using a permenant marker.
    - **Note:** If this point is not visible, remove sheath in small increments until it is visible (see video below).
    - **Note:** There must be at least 10 mm of bonded section for installing the IDC connectors. If there is less than 6 mm, remove more sheath to find a new transition point.
3. Make a mark 36 mm back from this transition point, using a permenant marker
    - **Note:** This value is the length of the split sections, taken from the datasheet (XXX)
4. Use a scalpel to remove the remaining sheath up to this mark.
5. Pull back the braid to expose the foil.
6. Use a scalpel to remove the foil, exposing the ribbon cable. Verify that the end of the sheath is aligned with the point where the ribbon cable changes from bonded to split (moving towards the end of the cable).

![adjusting-sheath-length](img/cable-preparation/adjusting-sheath-length.svg)

` placeholder for video `

## Installing the Connectors


![install-idc-connector](img/cable-preparation/install-idc-connector.svg)

## Sheath Surface Treatment for Bonding (Transducer End)

## Sheath Copper Coating for Shield Termination (Plug End)