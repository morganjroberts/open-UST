<p align="center">
  <img src="https://github.com/morganjroberts/open-UST/blob/main/docs/img/open-UST-logo-white-bg.png" width="50%">
</p>

# **open-UST:** An Open Source Manufacturing Framework for a Low-cost Ultrasound Tomography Research System.

There is a high barrier to entry for researchers starting ultrasound tomography (UST) experiments: UST hardware is not available off the shelf, and custom systems are expensive.
The goal of the open-UST project is to **lower the barrier to entry for experimental UST researchers**, by providing a manufacturing framework that allows end users to build their own UST transducers in-house.

<p align="center">
  <img src="https://github.com/morganjroberts/open-UST/blob/main/docs/img/home-image-nologo.png" width="75%">
</p>

open-UST is part of an ongoing research project, guided by three objectives:

1. High accessibility for end users.
2. Nominal acoustic behaviour that supports UST imaging research.
3. Low inter-element variation (IEV) in acoustic behaviour.

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

## Hardware Distribution and Documentation

To access the design and manufacture files, clone this repository locally:

```
git clone https://github.com/morganjroberts/open-UST
```

The design and manufacture files are located in the `hardware-distribution` directory.

For the accompanying manufacturing documentation, please visit [morganjroberts.github.io/open-UST](https://morganjroberts.github.io/open-UST/).

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

## Contact

open-UST is an ongoing research project from the [Biomedical Ultrasound Group](https://bug.medphys.ucl.ac.uk/) (University College London).

For questions, suggestions and feedback, please contact Morgan Roberts at [morgan.roberts.18@ucl.ac.uk](mailto:morgan.roberts.18@ucl.ac.uk).
