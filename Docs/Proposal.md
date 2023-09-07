# Classification of Medical Device Recalls 

- Author: Ruth Iang
- Prepared for UMBC Data Science Master Degree Capstone by Dr Chaojie (Jay) Wang
- https://github.com/DATA-606-2023-FALL-THURSDAY/Iang_Ruth
- Linkedin: https://www.linkedin.com/in/ruth-iang
- Link to your PowerPoint presentation file
- Link to your YouTube video

# Background
This project will focus on classifiying medical device recalls into 3 classes. A recall is when products are corrected or removed because they are in violation of Food and Drug Administration(FDA) laws.

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
- Data Shape: There are 17 columns and there are 2426 rows.
- Each row represents a medical device that is recalled by the FDA in violation of their laws.

# Data Dictionary

    1.) FEI Number: Integer64
    2.) Recalling Firm Name: Object, tells us the name of the firms 
    3.) Product Type: Object, tells us what firm the product belongs to
    4.) Product Classification: Object, represents how harmful the product is to the public
    5.) Status: Object, this column shows whether the recall is still going on
    6.) Distribution Pattern: Object, where the product is being distributed
    7.) Recalling Firm City: Object, the city where the product is being recalled 
    8.) Recalling Firm State: Object, the state where the prodcut is being recalled
    9.) Recalling Firm Country: Object, the country where the product is recalled
    10.) Center Classification Date: Datetime64[ns], the date when the product is classified
    11.) Reason for Recall: Object, reason why the product is in recall
    12.) Product Description: Object, describes the product 
    13.) Event ID: Integer64: Object, the id of the product when in recall
    14.) Event Classification: Object, the resulting classification
    15.) Product ID: Integer64, the id representing the product
    16.) Center: Object,shows the center where the devices is being recalled
    17.) Recall Details: Object, the product,and event details along with the history

# Target Variable/Label
Not all the columns will be used for the analysis or models because not all of them are eessential to the business question at hand. The column "Classification" will be 
the target variable. Classification I is has the worst damage to public health. Classification II represents mediocre health damage, and classification III does not lead to much problems. The medical device recalls will be classified into these categories.

# Potential Features/Predictors:
The column "Reason for Recall" is the feature variable for my model. The reasons listed for recalls will determine how severe the
potential or actual damage is to the community.
