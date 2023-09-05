# Classifying Medical Recalls 

- Author: Ruth Iang
- Prepared for UMBC Data Science Master Degree Capstone by Dr Chaojie (Jay) Wang
- https://github.com/DATA-606-2023-FALL-THURSDAY/Iang_Ruth
- Linkedin: https://www.linkedin.com/in/ruth-iang

# Background
This project will focus on classifiying medical device recalls into 3 classes. A recall is when products or corrected or removed because they are in violation of Food and Drug Administration(FDA) laws.

A recall takes place in order to protect the public health from products that has a risk of injury, deception or are defective. In order to determine the degree of health hazard
imposed by the products, FDA assigns the recalls into classification. Class I represents serious health result or death when exposed to the product or when using it. Class II
is when a temporary or reversible medical consequences will happen as a result of exposure or usage of the product. Class III represents cases when using or being in the presence
of the product does not lead to severe health problems. 

Medical device recalls is important because it advocates for the protection of public well being from devices that could cause
harm. And this is why my project will focus on classifiying FDA devices into their classification based on the provided reasons for recalls. Instead of manually classifiying these
devices, using Natural Language Processing and Machine Learning Algortithms will save time.

# Data
- Sources: This dataset is from FDA Open source data website.
- Data Size: The dataset is 245.6 MB.
- Data Shape: 
- Each row represents a medical device that is recalled by the FDA in violation of their laws.

# Data Types

# Target Variable/Label
Not all the columns will be used for the analysis or models because not all of them are eessential to the business question at hand. The column "Classification" will be 
the target variable. There are classification I, II, or III which represents the severity of har caused by the products.

# Potential Features/Predictors:
The column "Reason for Recall" is the feature variable for my model. The reasons listed for recalls will determine how severe the
potential or actual damage is to the community.
