## Data Description

We utilized Web crawling to acquire restaurant ratings from OpenTable.com, where both the overall rating and multi-criteria ratings are included. The major challenge in the process of data collection is identifying users. There are several anonymous ratings given by users. Namely, we are not able to identify a specific user or UserID from the Webpages. As a result, it is difficult to acquire dense ratings.

The OpenTable data set has been released on Kaggle.com. There are 19,536 ratings given by 1,309 users on 91 restaurants. In addition to the overall ratings, we have users' ratings on the restaurants from 4 criteria, including food quality, satisfaction of service and ambience, and the overall value of the picks. The ratings were given in the scale of 1 to 5.

The data set can be used for both traditional recommendations and multi-criteria recommendations. 

## Special Notes

- While working on web crawling for OpenTable.com, we found that HTML resources contained users' nickname instead of UserIDs. Occasionally, anonymous reviews used a default username, such as "Unknown user." To assign UserIDs, we treated the combination of username and city as a unique user. However, for entries with the default "Unknown user" username, we assigned the same ID. This explains why you might see multiple entries with the same <user, item> pair but different ratings.
- We provide the opentable_cleaned.csv file, where we removed duplicated entries and only include the last entry associated with the unique <user, item> pair in the data set.

## Citations

If you used this data for the purpose of research, please cite the following publications:

```
@article{zheng2024opentabledata,
title = {OpenTable data with multi-criteria ratings},
author={Zheng, Yong},
journal={arXiv preprint arXiv:2501.03072},
year={2024}
}
```
