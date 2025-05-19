---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

SlicerAutoscoperM (SAM) is a free, open source and multi-platform [3D Slicer](https://slicer.org) extension being developed for image-based 3D motion tracking of skeletal structures.

SAM includes modules for Pre-Processing, 3D tracking of structures captured via single, bi-, and multi-plane videoradiography ([Autoscoper](https://github.com/BrownBiomechanics/autoscoper)),3D registration of structures captured via 4DCT Sequential 3DCT or MRI ([Hierarchical 3D Registration](https://autoscoper.readthedocs.io/en/latest/tutorials/hierarchical-3d-registration.html)) and a Sample Autoscoper data Tracking Evaluation module.

<iframe src="https://drive.google.com/file/d/13AJJ0G3x-iVUNbyBQA6GJGcOfw9OV7Af/preview" width="640" height="480" allow="autoplay"></iframe>

## Current Features

* `N-plane Videoradiography` - Track 3D motion from 1 or more videoradiographs.
* `4DCT Registration` - Segmented 3DCT structures registered in each frame using [Elastix](https://elastix.dev/)
* `Ridged Body Kinematics` - Track the motion of ridged bodies in 3D space with 6 degrees of freedom.
* `Pre-Processing Module` - Generate segmentations and extract ridged bodies from 3DCT images.
* `Sample Data` - Download sample data to test SAM's features.

## What are we working on?

Below are some features currently under development:

* `Collision Detection` - Detect collisions between ridged bodies to inform the optimization process.
