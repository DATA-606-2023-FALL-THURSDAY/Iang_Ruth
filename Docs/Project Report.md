# Classification of Medical Device Recalls 

- Author: Ruth Iang
- Prepared for UMBC Data Science Masters Degree Capstone 
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
- Data Size: The dataset is 6.2 MB.
- Data Shape: There are 17 columns and there are 31012 rows.
- Each row represents a medical device that is recalled by the FDA in violation of their laws.
- The dataset has medical devices being recalled by the FDA for the last 11 years, from 2012 to October of 2023.

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
Not all the columns will be used for the analysis or models because not all of them are eessential to the business question at hand. The column "Event Classification" will be 
the target variable. "Event Classification" is how the products are classified into after doing an investigation. Classification I has the worst damage to public health. Classification II represents mediocre health damage, and classification III does not cause much health problems. The medical device recalls will be classified into these categories.

# Potential Features/Predictors:
The column "Reason for Recall" is the feature variable for my model. The reasons listed for recalls will determine how severe the
potential or actual damage is to the community.

# Explaratory Data Analysis
- Data Cleansing: I checked to see if there were null values and duplicate values in the dataset, which I later dropped.
- Data Preparation: Because this dataset is a text data, I normalized the feature column, "Reason for Recall" by tokeninizing, changing all letters to lowercase, keeping only stopwords, and stemming the words. This process keeps only the most important words in context of the topic for data preprocessing later on. Moreover, it helps to classify the devices more accurately..

- Visualizations:
  
  <img width="584" alt="image" src="https://github.com/DATA-606-2023-FALL-THURSDAY/Iang_Ruth/assets/98433448/af1bef98-97d6-453f-813c-cb436356e449">
- This pie chart shows us that most of the classifications in the datasets are classification II which means the health effects of many of these devices are mediocre. There are barely Class III which means many of the devices with classifications II aren't too many, or maybe they aren't too many complaints with devices in that category.

 <img width="800" alt="Screen Shot 2023-10-07 at 6 13 55 PM" src="https://github.com/DATA-606-2023-FALL-THURSDAY/Iang_Ruth/assets/98433448/a45813b6-3b39-4cee-893c-3ac12f8d05b8">

- The bar chart shows the same distribution as the pie chart above meaning there is imbalanced distribution between the classes.

<img width="593" alt="Screen Shot 2023-11-07 at 9 07 08 PM" src="https://github.com/DATA-606-2023-FALL-THURSDAY/Iang_Ruth/assets/98433448/a8eaefc5-1984-4a01-8395-f360cfe4e4e9">

- The WordCloud shows which words occur the most in the dataset. As shown, "may", "result","steril" and "compromis" are the words with the largest font. The size od the font is correlated with the frequency of the words in the feature varaible. And it makes sense in this context because such words would appear since the device would result in specific consequences. Also, many of the words are devices, kit, surgical items, procedures and so on. This shows what kind of medical devices are being recalled the most in the dataset.
