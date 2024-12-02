# Gaze4ASD

## Table of Contents
- [Overview](#overview)
- [Dataset Description](#dataset-description)
- [File Structure](#file-structure)
- [License](#license)

## Overview

The **Gaze4ASD** dataset contains eye gaze data for 132 TD children and 33 ASD children, who viewed 30 images selected by our **Image Selection Module**. These images were selected for their ability to elicit significant eye gaze differences between ASD and TD children.

These images and corresponding eye gaze data are provided to help researchers develop and validate models for automatic ASD screening based on visual saliency and gaze behavior.

Participants in the study were aged 3 to 7 years, with an average age of 4.54 years for the TD group and 5.04 years for the ASD group. ASD participants were clinically diagnosed with official medical documentation.

The eye gaze data were recorded using a **Tobii Pro Fusion eye tracker** with a 27-inch display (2560×1440 resolution, 120 Hz refresh rate). The participants sat 70 cm away from the screen. Each image was displayed for 3 seconds after the child focused on a child-friendly central icon, which helped capture their attention.

Eye tracker calibration was performed before data collection to ensure accurate gaze tracking.

## Dataset Description

This dataset is composed of the following components:

- **Images**: A set of 30 images that were used for eye gaze data collection.
- **Eye Gaze Data**: Raw eye gaze data collected from each participant during the viewing of the images.
- **Scanpath Data**: Processed eye gaze data that represents the sequential eye fixations made by each participant while viewing each image stimulus.
- **Saliency Maps**: Visual saliency maps generated from the scanpath data using a method described in the accompanying paper.

The dataset contains data on both ASD and TD children, with the goal of comparing gaze patterns between the two groups.

## File Structure

The dataset is organized as follows:

```
/Gaze4ASD
    /Image_Stimuli          # 30 images used for eye gaze data collection
    /ASD_rawdata            # Raw eye gaze data for ASD participants
    /TD_rawdata             # Raw eye gaze data for TD participants
    /ASD_Scanpath           # Scanpath data for ASD participants (sequence of fixations)
    /TD_Scanpath            # Scanpath data for TD participants (sequence of fixations)
    /ASD_Saliency           # Visual saliency maps for ASD children (generated from scanpath)
    /TD_Saliency            # Visual saliency maps for TD children (generated from scanpath)
```

## License

This dataset is provided under the [MIT License](https://opensource.org/licenses/MIT).

