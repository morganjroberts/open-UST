# Array Mounting Plate

<p align="center">
  <img src="https://github.com/morganjroberts/open-UST/blob/main/docs/img/2D-ring-array-mounting-plate/array-mounting-plate.png" width="50%">
</p>

## Mounting Plate Design
- The original array mounting plate CAD object is found within the `transducer-module.f3d` source file, since the hole layout references the transducer geometry and parameters.
- `array-mounting-plate.step` and `array-mounting-plate.f3d` are also included but have no timeline history.

## Mounting Plate Manufacture
The array mounting plate uses precision-drilled holes to align the transducer modules.

- We CNC drilled this part, and the g-code was created using the "manufacture" tool in Fusion 360. The toolpaths are included in the `array-mounting-plate.f3d` file.
- Alternatively this part could be manually drilled. A to-scale `array-mounting-plate.pdf` file is included as a template, which could be printed at 100% size to assist with the hole layout.
- Alternatively, a laser cutter could be used to engrave the hole layout, using the `array-mounting-plate.dxf` file, and then the holes could be drilled.
- Fully laser cutting the holes is not recommended, since a drill bit is more precise.

## Rails and Brackets

- We mounted the array using aluminium extrusion rails and 3D-printed brackets.
- Designed for a rail spacing of 500 mm: [Precision Acoustics standard tank](https://www.acoustics.co.uk/product/ums-tank-specification/)
- The array mounting bracket CAD object is found within the `transducer-module.f3d` source file.
- `array-mounting-bracket.step` and `array-mounting-bracket.stl` are also included.

