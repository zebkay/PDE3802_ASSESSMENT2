# 3D Object Pose Estimation with Raspberry Pi + ROS (PDE3802 Assessment 2)

> **Status:** work in progress. Sections marked _TODO_ are filled in as the project develops.

## 1. What this is

A computer-vision system running on a Raspberry Pi with a PiCamera that detects
five physical objects and estimates their 3D pose relative to the camera:

- **2 objects with ArUco tags**: pose from the tag.
- **3 objects without tags**: detection + pose from known object size.

Each object's pose is published to ROS as its own uniquely named TF frame
(parent: the camera frame) and visualised in RViz.

_TODO: one-paragraph summary of the final approach and results._

## 2. Team and responsibilities

| Name | Student ID | GitHub | Responsibilities |
| ---- | ---------- | ------ | ---------------- |
| Kay Bugingo | M00971312 | zebkay | _TODO_ |
| _TBD_ | | | _TODO_ |

## 3. Objects

| # | Object | Type | Tag ID / class | Real size (m) | TF frame |
| - | ------ | ---- | -------------- | ------------- | -------- |
| 1 | _TODO_ | ArUco | | | `object_1_frame` |
| 2 | _TODO_ | ArUco | | | `object_2_frame` |
| 3 | _TODO_ | Vision | | | `object_3_frame` |
| 4 | _TODO_ | Vision | | | `object_4_frame` |
| 5 | _TODO_ | Vision | | | `object_5_frame` |

## 4. Hardware and software

- Raspberry Pi: _TODO_
- Camera: _TODO_
- OS / ROS version: _TODO_
- Python: _TODO_

## 5. Installation

_TODO_

```
git clone https://github.com/zebkay/PDE3802_ASSESSMENT2.git
cd PDE3802_ASSESSMENT2
```

## 6. Camera calibration

_TODO: how to print the checkerboard, capture images, run the calibration script._

## 7. How to run

_TODO: exact commands, e.g. launch the node, open RViz with `rviz/` config._

## 8. Expected output

_TODO: what appears in the terminal, which TF frames appear in RViz, screenshots in `docs/figures/`._

## 9. Troubleshooting

| Problem | Fix |
| ------- | --- |
| _TODO_ | _TODO_ |

## 10. Results and limitations

_TODO: accuracy, tested backgrounds, known failure cases._

## 11. Project layout

```
config/        configuration (tag size, object sizes, thresholds)
calibration/   camera calibration output (raw photos are git-ignored)
src/           detection, pose estimation and ROS nodes
scripts/       helper scripts (calibration capture, tag generation)
rviz/          saved RViz configuration
models/        trained models (download separately, see README)
data/          dataset notes / manifest (images not stored in Git)
docs/          figures and notes for the presentation
tests/         unit tests
```
