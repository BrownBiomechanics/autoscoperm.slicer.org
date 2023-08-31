---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

SlicerAutoscoperM (SAM) is a free, open source and multi-platform [3D Slicer](https://slicer.org) extension being developed for image-based 3D motion tracking of skeletal structures.

SAM is a single software package based on [Autoscoper](https://github.com/BrownBiomechanics/autoscoper) that enables the 3D tracking of structures within multiple imaging modalities including single, bi-, and multi-plane videoradiography, sequential CT volume images, 4DCT image volumes sets, and MRI volume sets. SAM will be built by updating and refining Autoscoper which is a bi-plane video radiography image registration software developed at Brown University, and then integrating it into the 3DSlicer ecosystem.

![Autoscoper Main Window](https://github.com/BrownBiomechanics/Autoscoper/releases/download/docs-resources/tutorial_AutoscoperMainWindow.png)

## Current Features

* `N-plane Videoradiography` - Track 3D motion from 1 or more videoradiographs.
* `Ridged Body Kinematics` - Track the motion of ridged bodies in 3D space with 6 degrees of freedom.
* `Pre-Processing Module` - Generate segmentations and extract ridged bodies from 3DCT images.
* `Sample Data` - Download sample data to test SAM's features.

## What are we working on?

Below are some features currently under development:

* `Collision Detection` - Detect collisions between ridged bodies to inform the optimization process.
* `Pre-Processing Module` - Generate radiographic projections from 3D and 4D CT images.