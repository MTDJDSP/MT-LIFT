# MT-LIFT
*MT-LIFT* is a large-scale and unbiased dataset collected from two months of coupon marketing scenarios for food delivery in the Meituan App, [Meituan (美团)](https://www.meituan.com).  **It is the first unbiased industrial dataset featuring multiple treatments and comprehensive chain labels (click and conversion) information!** 

## Overview:
To eliminate the impact of confounding factors on uplift modeling, we collect it from randomized controlled trials, where treatments were randomly assigned to ensure consistent potential distribution between the treatment and control groups. To protect data privacy, we have implemented both anonymization and desensitization techniques on the features. 

You can download the dataset from the [Google drive](https://drive.google.com/file/d/18Zj-TW-MP_ntbiru6nRBseMxSwCKB3zq/view?usp=drive_link).

MT-LIFT provides a rich dataset comprising of extensive feature and label information, making it a valuable resource for various research areas. It particularly supports the following research objectives:

- Click-through rate (CTR) prediction.
- Conversion rate (CVR) prediction.
- Uplift modeling.
- Joint modeling of click and conversion.

Compared with other datasets, MT-LIFT has the following advantages:
- ✅ We collected it from an unbiased treatment assignment, ensuring that the user response changes is solely influenced by the treatment.
- ✅ It has abundant features and provides ample opportunities for various algorithms to extract valuable information.
- ✅ It has multiple treatments, offering additional information for uplift modeling and exploring the effects of differential interventions.
- ✅ We collected it from the impression space, including comprehensive chain information for accurate analysis of user responses.

If you find it helpful, please cite our paper:
 [![LINK](https://img.shields.io/badge/-Paper%20Link-lightgrey)](https://arxiv.org/submit/5387809/view)

```
@inproceedings{huang2024,
  title = {Entire Chain Uplift Modeling with Context-Enhanced Learning for Intelligent Marketing},
  author = {Yinqiu Huang, Shuli Wang, Min Gao, Xue Wei, Changhao Li, Chuan Luo, Yinhua Zhu, Xiong Xiao and Yi Luo	},
  doi = {10.1145/3511808.3557624}
}
```
----


## Data Descriptions

The file structure of the dataset is listed as follows:
##### MT-LIFT   (10.49GB)

  ```shell
  MT-LIFT
  ├── train.csv (8.64GB)
  └── test.csv  (1.85GB)
  ```

Data fields:
There are 102 fields in total, of which 99 are features(f0~f98).
  ```
| Field Name:    | Description                                                  |
| -------------- | ------------------------------------------------------------ |
| click          | The click label.                                             | 
| conversion     | The conversion label.                                        | 
| treatment      | The treatment label. In the range of [0, 4]                  |
| f0-f98         | The features.                                                | 

