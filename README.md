# SS2025 : Setup and Execution Notes
## Pre-Requesit:
- Python 3.11.*
- YOLOv11
- CUDA
- Torch

## Running Scripts
- Install deps. by running following command on the root directory:

    `
        pip install .
    `
- Download and unzip dataset from ASDF repo. and place them in `./datasets-downloaded` folder.

https://olymp.mixality.de/?launchApp=SYNO.SDS.Drive.Application#file_id=877954175831421891

- To generate RGBD Pose training data, run the script `./Helper_scripts/bproc_to_rgbd-yolo_pose.py)`.
  
  The script is going to generate both training data `./datasets/rgbd_pose/NanoVise/train` and validation data `./datasets/rgbd_pose/NanoVise/val`.
  ### note
  Note that this script is going to generate the images and lables to be used later in YOLO training. So it will take arround 30 mins to execute. 

- Ensure that following folder has been created `./datasets/rgbd_pose/NanoVise/*`
- 


# ASDF: Assembly State Detection Utilizing Late Fusion by Integrating 6D Pose Estimation

Hannah Schieber*, Shiyu Li†, Niklas Corell‡, Philipp Beckerle+, Julian Kreimeier¶, and Daniel Roth∥

Technical University of Munich
School of Medicine and Health
Department Clinical Medicine
Machine Intelligence in Orthopedics
Clinic for Orthopedics and Sports Orthopedics*,†,¶,||

Friedrich-Alexander-Universitat¨
Erlangen-Nurnberg (FAU) ¨
Erlangen, Germany*,†,‡,+

## Dataset

# Eval and Training Sample
[ASDF Evaluation Dataset + Corner Clamp Base](https://zenodo.org/records/11188134)

## Training
[Hand Screw Clamp](https://zenodo.org/records/11206073)


[Training Set - NanoVise part 2](https://zenodo.org/records/11194439)

[Training Set - NanoVise part 1](https://zenodo.org/records/11194431)

[Training Set - Corner Clamp Part 1](https://zenodo.org/records/11194297)

[Training Set - Corner Clamp Part 2 - Geared Caliper Base](https://zenodo.org/records/11194303)

The yolo part of this work is from Ultralytics

YOLO is under the following license:
- **AGPL-3.0 License**: This [OSI-approved](https://opensource.org/licenses/) open-source license is ideal for students and enthusiasts, promoting open collaboration and knowledge sharing. See the [LICENSE](https://github.com/ultralytics/ultralytics/blob/main/LICENSE) file for more details.
