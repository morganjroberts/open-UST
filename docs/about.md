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

1. High accessibility for end users.
1. Nominal acoustic behaviour that supports UST imaging research.
1. Low inter-element variation (IEV) in acoustic behaviour.

This work will support researchers to build their own UST systems in house, accelerating progress towards fast and accurate UST imaging.

This documentation is part of the open-source hardware distribution.

## Features

- **Simple equipment requirements:** No specialist equipment required, only a 3D-printer, vacuum chamber and standard workshop tooling.
- **Low material cost:** ~£2k (excluding DAQ hardware) for a 256-element system.
- **Modular:** Both 2D and 3D imaging setups can be configured. 
- **Low interelement variation**: Recent testing showed that the individual sensing elements have uniform acoustic behaviour.
- **Other:**
    - Fully waterproof
    - Electromagnetically shielded
    - Transducer modules feature threaded mounting points for repeatable positioning
    - Includes option for a modular interface with the ITT Cannon DL5-260P connector (compatible with Verasonics)

## Citing open-UST

Please cite this article if you use open-UST in your research:

```
@article{roberts2023open,
  title     = {open-UST: An Open-Source Ultrasound Tomography Transducer Array System},
  author    = {Roberts, Morgan and Martin, Eleanor and Brown, Michael D and Cox, Ben T and Treeby, Bradley E},
  journal   = {IEEE Transactions on Ultrasonics, Ferroelectrics, and Frequency Control},
  year      = {2023},
  publisher = {IEEE},
  doi       = {10.1109/TUFFC.2023.3280635}
}
```