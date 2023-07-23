# SRI-Graph: A Novel Scene-Robot Interaction Graph for Robust Scene Understanding

This is the implementation of the paper SRI-Graph: A Novel Scene-Robot Interaction Graph for Robust Scene Understanding (ICRA 2023). This repository will be updated soon.

# Introduction

We propose an annotation tool LabelImg-Rel (based on [LabelImg](https://github.com/heartexlabs/labelImg)) for convenient and efficient relationship annotation. We release a new dataset named 3DRF-Pos, it contains the RGB images and corresponding 3D positions of the robot manipulator during the real-world 3D robot-feeding teleoperation task.

# LabelImg-Rel

## Installation

Python 3 or above are required.

```
pip3 install PyQt5 lxml
```

## Launch Annotation Tool

```
cd LabelImg-Rel
python labelImg-rel.py
```
Click the button "open dir" for choosing the dataset folder, For the annotation of bounding boxes, please follow the instruction of [LabelImg](https://github.com/heartexlabs/labelImg).
To label the relationships, click the subject bounding box, object bounding box, and the button "Create predicate" in the left column.

## Annotate on Custom Images/Datasets

Change `predefined_classes.txt` (predefined object classes) and `predefined_predicates.txt` (predefined relationship classes) in the folder `LabelImg-Rel/data`.

# 3DRF-Pos Dataset


# Citation

If you find our work helpful, please consider citing:

```bib
@inproceedings{yang2023sri,
  title={Sri-graph: A novel scene-robot interaction graph for robust scene understanding},
  author={Yang, Dong and Xu, Xiao and Xiong, Mengchen and Babaians, Edwin and Steinbach, Eckehard},
  booktitle={2023 IEEE International Conference on Robotics and Automation (ICRA)},
  pages={8171--8178},
  year={2023},
  organization={IEEE}
}
```

# Acknowledgements

Our codes are built on top of some open-source projects. Thanks for their contributions:

[Scene Graph Benchmark in Pytorch](https://github.com/KaihuaTang/Scene-Graph-Benchmark.pytorch)

[LabelImg](https://github.com/heartexlabs/labelImg)
