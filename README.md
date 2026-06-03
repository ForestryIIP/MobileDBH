# MobileDBH Field Dataset

## Overview

This dataset contains field-collected tree images and corresponding DBH (Diameter at Breast Height) measurements used in the paper:

**MobileDBH: Estimating Tree Diameter at Breast Height from Smartphone Images Using a Lightweight Diffusion Depth Network for Field Tree Phenotyping**

## Data Collection

- **Location**: Experimental Forest, Beijing Forestry University, Beijing, China
- **Date**: 2025
- **Number of trees**: 20
- **DBH range**: 11.46 cm to 30.86 cm

## Measurement Method

Tree circumference was measured manually at breast height (1.3 m) using a tape measure and converted to DBH using the formula:

DBH = Circumference / π

## Dataset Structure

```
MobileDBH-FieldDataset/
├── README.md
├── images/
│   ├── img_1.jpg
│   ├── img_2.jpg
│   ├── img_3.jpg
│   ├── img_4.jpg
│   └── img_5.jpg
└── annotations.csv
```

## Annotations

The file `annotations.csv` contains the following fields:

| Field | Description |
|-------|-------------|
| image | Source image filename |
| position | Position of the tree in the image, counted from right to left (1 = rightmost) |
| dbh_cm | DBH converted from circumference measurement (cm) |

## Image Contents

| Image | Position (right to left) | DBH (cm) |
|-------|--------------------------|----------|
| img_1 | 1 | 23.12 |
| img_1 | 2 | 16.24 |
| img_1 | 3 | 21.31 |
| img_1 | 4 | 23.09 |
| img_2 | 1 | 20.38 |
| img_2 | 2 | 15.85 |
| img_2 | 3 | 19.43 |
| img_2 | 4 | 19.88 |
| img_3 | 1 | 15.13 |
| img_3 | 2 | 24.68 |
| img_3 | 3 | 19.42 |
| img_3 | 4 | 11.46 |
| img_4 | 1 | 15.96 |
| img_4 | 2 | 24.26 |
| img_4 | 3 | 15.44 |
| img_4 | 4 | 30.86 |
| img_5 | 1 | 24.89 |
| img_5 | 2 | 30.86 |
| img_5 | 3 | 24.26 |
| img_5 | 4 | 15.96 |

## Notes

- Each image contains multiple trees.
- Tree positions are recorded from right to left as they appear in the image. For example, position 1 refers to the rightmost tree, position 2 refers to the second tree from the right, and so on.
- Tree 5 was excluded from evaluation due to anomalous intermediate results.


## Citation

If you use this dataset, please cite our paper:


## Contact

For data requests, please contact the corresponding author:
Haiyan Zhang (zhyzml@bjfu.edu.cn)
