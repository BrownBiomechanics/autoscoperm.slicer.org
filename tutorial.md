---
layout: page
title: Tutorial
permalink: /tutorial/
---
# Tutorial
This tutorial will walk you through the steps to use SAM to track a 3D motion of a skeletal structure from a single bi-plane video radiography image set.

## Prerequisites
SAM is a 3D Slicer extension. Therefore, you will need to install 3D Slicer first. The **preview** version of Slicer is required, which can be found [here](https://download.slicer.org/). SAM is currently only available for Windows and Linux operating systems. MacOS support is planned for the future.

## Installation
SAM is available as a 3D Slicer extension. You can install it from the 3D Slicer extension manager. To open the extension manager, go to `View` -> `Extension Manager` in the main menu. In the extension manager, search for `AutoscoperM` and click `Install` to install SAM. Once SAM is installed, switch to the `AutoscoperM` module by clicking `Modules` -> `AutoscoperM` in the main menu.

## Loading Sample Data
Once the module is loaded, you can launch the module by clicking the `Launch Autoscoper` button. The module will open in a separate window.

SAM ships with several sample data sets. To load a sample data set, go to `Help` -> `Open Sample - Wrist`. There are also datasets for the Knee and the Ankle. You can load them by going to `Help` -> `Open Sample - Knee` or `Help` -> `Open Sample - Ankle`. Once the data is loaded, you should see the following screen:

![Sample Data Loaded](https://github.com/BrownBiomechanics/Autoscoper/releases/download/docs-resources/tutorial_SampleLoaded.png)

To zoom in on the radiographs and see the details, you can use `Control + Mouse Wheel` to zoom in and out. To adjust the position of the radiographs, you can use `Control + Left Mouse Button` to pan the radiographs.

## Tracking a Skeletal Structure

### Aligning a Volume
SAM tracks a skeletal structure by aligning a volume to a set of bi-plane radiographs. To align a volume, start by selecting the volume you wish to align from the volumes list in the lower left corner of the screen. In this case, we will align the radius or the `rad_dcm_cropped` volume. Once the volume is selected, you can move your mouse over to one of the radiograph images and use the `Left Mouse Button` to move the volume around. 

You can press `E` to switch to rotation mode, or `W` to go back to translation mode. If need you can press `D` to move the location of the pivot point. Pressing `C` will perform the optimization on the current frame, this can be useful for snapping the volume to the radiographs. 

You may find it easier to align the volume with one of the radiographs first, then make sure the volume is aligned with all the radiographs.

![Aligned with the right radiograph](https://github.com/BrownBiomechanics/Autoscoper/releases/download/docs-resources/tutorial_AlignedWithRight.png)

![Aligned with both radiographs](https://github.com/BrownBiomechanics/Autoscoper/releases/download/docs-resources/tutorial_AlignedWithBoth.png)

### Tracking the volume
Once the volume is aligned with the radiographs, you can press the `Tracking Dialog` button to open the tracking dialog. The dialog will look like this:

![Tracking Dialog](https://github.com/BrownBiomechanics/Autoscoper/releases/download/docs-resources/tutorial_TrackingDialog.png)

The dialog has several options. The first option is the `Tracking Range` which allows you to specify the range of frames you wish to track. The default is to track all the frames in order. The second option is `Intial Guess`, changing this will change how the intial position of the volume is determined. The default is to use the position of the volume in current frame. The third option is `Optmiziation method`, you can choose between partical swarm optmiziation (PSO) or downhill simplex. The default is PSO. You can also specifiy the number of time you want the optmization to run on each frame. The default is 1. The fourth option is `PSO Algorithm Parameters`, you can change the parameters for the optmization here. The default values are usually good enough. The last option is `Cost Function`, you can choose between the normalized cross correlation (NCC) or the sum of absolute differences (SAD). The default is NCC.

Once you have set the options, you can press the `Ok` button to start tracking. The tracking will take a while to complete, and trials with lots of frames will take even longer. Once the tracking is complete, the dialog will close.

### Viewing the tracking results
Once the tracking is complete, you can view the tracking results by moving the slider at the bottom of the screen.

![Tracking Results](https://github.com/BrownBiomechanics/Autoscoper/releases/download/docs-resources/tutorial_tracked.gif)

You can also view the tracking results in the 3D view by going to `View` -> `Show World View` in the main menu. You can use `Control + Middle Mouse Button` to pan the 3D view, `Control + Left Mouse Button` to rotate the 3D view, and `Control + Right Mouse Button + Drag` to zoom in and out.

![World View](https://github.com/BrownBiomechanics/Autoscoper/releases/download/docs-resources/tutorial_WorldView.png)
