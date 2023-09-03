# Background
This project will focus on classifiying medical device recalls into 3 classes. A recall is when products or corrected or removed because they are in violation of Food and Administration(FDA) laws.
A recall takes place in order to protect the public health from products that has a risk of injury, deception or are defective. In order to determine the degree of health hazard
imposed by the products, FDA assigns the recalls into classification. Class I represents serious health result or death when exposed to the product or when using it. Class II
is when a temporary or reversible medical consequences will happen as a result of exposure or usage of the product. Class III represents cases when using or being in the presence
of the product does not lead to severe health problems. Medical device recalls is important because it advocates for the protection of public well being from devices that could cause
harm. And this is why my project will focus on classifiying FDA devices into their classification based on the provided reasons for recalls. Instead of manually classifiying these
devices, using Natural Language Processing and Machine Learning Algortithms will save time.

# Data
The data is taken from the officical FDA data website. The size is currently 50.5KB when using data from May to the begining of September, 2023. Depending on the data analysis,
more data might be added later on. There are 25 columns, and 258 rows. Each row represents a device that is recalled by the FDA. Most columns are type object with Event ID being type
integer. Not all the columns will be used for the analysis or models because not all of them are eessential to the business quetrion at hand. The column classification will be 
the target variable, and the column Reason for Recall is feature variables for my models. 
