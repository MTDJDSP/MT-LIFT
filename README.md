# MT-LIFT
*MT-LIFT* is a large-scale and unbiased dataset collected from two months of coupon marketing scenarios for food delivery in the Meituan App, [Meituan (美团)](https://www.meituan.com).  **It is the first unbiased industrial dataset featuring multiple treatments and comprehensive chain label (click and conversion) information!** 

## Overview:
To eliminate the impact of confounding factors on uplift modeling, we collect it from randomized controlled trials, where treatments were randomly assigned to ensure consistent potential distribution between the treatment and control groups. MT-LIFT provides a rich dataset comprising of extensive feature and label information, making it a valuable resource for various research areas. It particularly supports the following research objectives:
-Click-through rate (CTR) prediction: This task involves estimating the probability of users clicking on items. CTR prediction is widely applied in Internet companies and e-commerce platforms.
-Conversion rate (CVR) prediction: Essential for ranking systems in industrial applications like online advertising and recommendation engines, CVR prediction aims to estimate the likelihood of users completing a desired action, such as making a purchase.
-Uplift modeling: This technique aims to accurately identify the difference in a user's response with and without a specific treatment. It outputs an uplift score, which represents the increase in conversion rate resulting from a particular intervention, such as offering a specific coupon.
