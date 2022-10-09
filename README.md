
<p align="center">
  <img src="https://github.com/morganjroberts/open-UST/blob/main/docs/img/open-UST-logo-white-bg.png" width="50%">
</p>

# **open-UST:** An Open Source Manufacturing Framework for a Low-cost Ultrasound Tomography Research System.

There is a high barrier to entry for researchers starting ultrasound tomography (UST) experiments: UST hardware is not available off the shelf, and custom systems are expensive.
The goal of the open-UST project is to **lower the barrier to entry for experimental UST researchers**, by providing a manufacturing framework that allows end users to build their own UST transducers in-house.

<p align="center">
  <img src="https://github.com/morganjroberts/open-UST/blob/main/docs/img/home-image-nologo.png" width="100%">
</p>

open-UST is part of an ongoing research project, guided by three objectives:

1. Design a low cost UST research system and manufacture it in-house.
1. Measure its acoustic performance and imaging capability, and assess its overall suitability as a tool for the UST research community.
1. Release the design as an open-source hardware distribution.

If successful, this work will support researchers to build their own UST systems in house, accelerating progress towards fast and accurate UST imaging.

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

## Hardware Distribution and Documentation

To access the design and manufacture files, clone this repository locally:

```
git clone https://github.com/morganjroberts/open-UST
```

The design and manufacture files are located in the `hardware-distribution` directory.

For the accompanying manufacturing documentation, please visit [morganjroberts.github.io/open-UST](https://morganjroberts.github.io/open-UST/).

## Citing open-UST

open-UST will shortly be published in a journal paper. Currently, please cite this repository if you use open-UST in your research:

```
@misc{roberts2022_open-UST,
	title          =    { open-UST: An Open Source Manufacturing Framework for a Low-cost Ultrasound Tomography Research System  },
	author         =    { Morgan Roberts and Eleanor Martin and Michael Brown and Ben Cox and Bradley Treeby },
	year           =    { 2022 },
	url            =    { https://github.com/morganjroberts/open-UST }
}
```

## Contact
open-UST is an ongoing research project from the [Biomedical Ultrasound Group](https://bug.medphys.ucl.ac.uk/) (University College London).

For questions, suggestions and feedback, please contact Morgan Roberts at [morgan.roberts.18@ucl.ac.uk](mailto:morgan.roberts.18@ucl.ac.uk).


