# MT-LIFT
*MT-LIFT* is a large-scale and unbiased dataset collected from two months of coupon marketing scenarios for food delivery in the Meituan App, [Meituan (美团)](https://www.meituan.com).  **It is the first unbiased industrial dataset featuring multiple treatments and comprehensive chain labels (click and conversion) information!** 

## Overview:
To eliminate the impact of confounding factors on uplift modeling, we collect it from randomized controlled trials, where treatments were randomly assigned to ensure consistent potential distribution between the treatment and control groups. To protect data privacy, we have implemented both anonymization and desensitization techniques on the features. 

You can download the dataset from the [Google drive](https://drive.google.com/file/d/1dslFa9EGrVVoO_040ZYM16cIH-SKDuss/view?usp=drive_link) | [Baidu drive](https://pan.baidu.com/s/1YmE5g-Y71ULNptiWqpToPA?pwd=06nb).

MT-LIFT comprising of extensive feature and label information, making it a valuable resource for various research areas. It particularly supports the following research:

- Click-through rate (CTR) prediction.
- Conversion rate (CVR) prediction.
- Joint modeling.
- Uplift modeling.
  
Compared with other datasets, MT-LIFT has the following advantages:
- ✅ We collected it from an unbiased treatment assignment, ensuring consistent potential distribution between the treatment and control groups.
- ✅ It has abundant features and provides ample opportunities to extract valuable information.
- ✅ It has multiple treatments for exploring the effects of differential interventions.
- ✅ We collected it from the impression space, including comprehensive chain information for accurate analysis of user responses.

If you find it helpful, please cite our paper:
 [![LINK](https://img.shields.io/badge/-Paper%20Link-lightgrey)](https://arxiv.org/abs/2402.03379)

```
@article{huang2024entire,
  title={Entire Chain Uplift Modeling with Context-Enhanced Learning for Intelligent Marketing},
  author={Huang, Yinqiu and Wang, Shuli and Gao, Min and Wei, Xue and Li, Changhao and Luo, Chuan and Zhu, Yinhua and Xiao, Xiong and Luo, Yi},
  journal={arXiv preprint arXiv:2402.03379},
  year={2024}
}
```
----


## Data Descriptions

The file structure of the dataset is listed as follows:
##### MT-LIFT  

  ```shell
  MT-LIFT
  ├── train.csv 
  └── test.csv  
  ```

Data fields:
There are 102 fields in total, of which 99 are features(f0~f98).

  ```
  | Field Name:    | Description                                                  |
  | -------------- | ------------------------------------------------------------ |
  | click          | The click label.                                             | 
  | conversion     | The conversion label.                                        | 
  | treatment      | The treatment label. In the range of [0, 4].                 |
  | f0-f98         | The features.                                                |


The statistics of MT-LIFT:

  ```shell
  | size           | 5,541,842.                                                   | 
  | Features       | 99.                                                          | 
  | treatment      | The treatment label. In the range of [0, 4]                  |
  | f0-f98         | The features.                                                | 

