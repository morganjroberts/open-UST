# About

##  Ultrasound Tomography and Breast Cancer
- Breast cancer screening with mammograms reduces mortality, but false negatives can occur for people with high breast density, and over-diagnosis causes harm in healthy people.
- Ultrasound Tomography (UST) is an emerging but promising modality that produces images of the sound-speed and acoustic-absorption distributions in breast tissue. These properties are useful biomarkers for classifying healthy and abnormal tissue types.
- UST could perform better than mammography, since it generates 3D images instead of 2D images.
- UST is also non-ionising, requires no painful breast compression, and is cheaper than MRI.

## Challenges in UST
- Widespread clinical adoption requires shorter data acquisition and image reconstruction times, while maintaining accuracy.
- Work towards this goal means that new methods must be tested experimentally.
- There is a high barrier to entry for researchers starting UST experiments: UST hardware is not available off the shelf, and custom systems are expensive.

## open-UST
**The goal of the open-UST project is to lower the barrier to entry for experimental UST researchers.**
This research project is guided by three objectives:

1. Design a low cost UST research system and manufacture it in-house.
1. Measure its acoustic performance and imaging capability, and assess its overall suitability as a tool for the UST research community.
1. Release the design as an open-source hardware distribution.

If successful, this work will support researchers to build their own UST systems in house, accelerating progress towards fast and accurate UST imaging.

This documentation is part of the open-source hardware distribution.

## Features

- **Simple end-user requirements:** No specialist equipment required, only a 3D-printer and vacuum chamber.
- **Low material cost:** ~£2,500 (excluding DAQ hardware) for a 256-element system.
- **Modular:** Both 2D and 3D imaging setups can be configured. 
- **Low interelement variation**: Recent testing showed that the individual sensing elements have uniform acoustic behaviour.
- **Other:**
    - Fully waterproof
    - Electromagnetically shielded
    - Modules feature threaded mounting points for repeatable positioning
    - Includes option for a modular interface with the ITT Cannon DL5-260P connector (compatible with Verasonics)

## Citing open-UST

open-UST will shortly be published in a journal paper. Currently, please cite the GitHub repository if you use open-UST in your research:

```
@misc{roberts2022_open-UST,
	title          =    { open-UST: An Open Source Manufacturing Framework for a Low-cost Ultrasound Tomography Research System  },
	author         =    { Morgan Roberts and Eleanor Martin and Michael Brown and Ben Cox and Bradley Treeby },
	year           =    { 2022 },
	url            =    { https://github.com/morganjroberts/open-UST }
}
```