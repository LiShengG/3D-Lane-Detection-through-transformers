# 3D-Lane-Detection-through-transformers

🙂 **Our project code will be published soon**

This repository is an official implementation of the paper *3D Lane Detection through transformers*

Our methed architecture is as following
![ous model](https://github.com/LiShengG/3D-Lane-Detection-through-transformers/blob/main/model.png)

Main comparison with state-of-the-art methods on ![synthetic dataset](https://github.com/yuliangguo/Pytorch_Generalized_3D_Lane_Detection).
The dataset is divided into three parts.(1)balances scenes; (2)rarely observed; (3)visual variations

- (1)balances scenes

| Method      | lane    |      |       |       |  Cneter lane |      |       |       |
|:-----------:|:-------:|:----:|:-----:|:-----:|:------------:|:----:|:-----:|:-----:|
|             | F-Score | AP   | z-e   | zz -e | F-Score      | AP   | z -e  | zz-e  |
| 3D-LaneNet  | 86.4    | 89.3 | 0.015 | 0.202 | 89.5         | 91.4 | 0.015 | 0.179 |
| Gen_LaneNet | 88.1    | 90.1 | 0.012 | 0.214 | 90.8         | 92.6 | 0.011 | 0.176 |
| ours        | **92.5** | **90.4** | **0.01**  | 0.239 | **95.4**  | **93.3** | **0.01**  | 0.219 |

- (2)rarely observed

| Method      | lane    |      |       |       |  Cneter lane |      |       |       |
|:-----------:|:-------:|:----:|:-----:|:-----:|:------------:|:----:|:-----:|:-----:|
|             | F-Score | AP   | z-e   | zz -e | F-Score      | AP   | z -e  | zz-e  |
| 3D-LaneNet  | 72      | 74.6 | 0.039 | 0.521 | 77           | 80   | 0.04  | 0.557 |
| Gen_LaneNet | 78      | 79   | 0.03  | 0.539 | 79.5         | 80.6 | 0.026 | 0.547 |
| ours        | **85.2** | **83.5** | **0.027**| 0.617 | **87.1** | **84.8** | 0.028 | 0.648 |

- (3)visual variations

| Method      | lane    |      |       |       |  Cneter lane |      |       |       |
|:-----------:|:-------:|:----:|:-----:|:-----:|:------------:|:----:|:-----:|:-----:|
|             | F-Score | AP   | z-e   | zz -e | F-Score      | AP   | z -e  | zz-e  |
| 3D-LaneNet  | 72.5    | 74.9 | 0.032 | 0.23  | 75.5         | 77.7 | 0.03  | 0.227 |
| Gen_LaneNet | 85.3    | 87.2 | 0.015 | 0.232 | 88.2         | 90   | 0.015 | 0.187 |
| ours        | **90.1**|**88.2**| **0.012**| 0.284 | **93.2** | **91.3** | **0.012** | 0.263 |
