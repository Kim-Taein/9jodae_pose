# 9jodae_OmniPose

<p align="center">
  <img src="https://people.rit.edu/bm3768/images/omnipose.png" title="OmniPose Architecture">
  Figure 1: OmniPose framework for multi-person pose estimation. The input color image of dimensions (HxW) is fed through the improvedHRNet backbone and WASPv2 module to generate one heatmap per joint, or class.
</p><br />

<p align="center">
  <img src="https://people.rit.edu/bm3768/images/WASPv2.png" width=1000 title="WASPv2 module"><br />
  Figure 2: WASPv2 Module.
</p><br />

Examples of the OmniPose architecture for Multi-Person Pose Estimation are shown in Figures 3.<br />

<p align="center">
  <img src="https://people.rit.edu/bm3768/images/samples.png" width=1000 title="WASP module"><br />
  Figure 3: Pose estimation samples for OmniPose.
  <br /><br />
  
</p><br />


**Data preparation:**

**COCO**

    ${OMNIPOSE_ROOT}
    |-- data
    `-- |-- coco
        `-- |-- annotations
            |   |-- person_keypoints_train2017.json
            |   `-- person_keypoints_val2017.json
            `-- images
                |-- train2017.zip
                `-- val2017.zip
                
**MPII**

    ${OMNIPOSE_ROOT}
    |-- data
    `-- |-- mpii
        `-- |-- annot
            |   |-- train.json
            |   `-- valid.json
            `-- images

#### Training
```
bash run_train.sh
```

#### Testing
```
bash run_demo.sh
```
