## ANALYZING ROAD SAFETY & TRAFFIC DEMOGRAPHICS IN THE UK (Multi-class Classification)

### SUMMARY
Here, I am aim to analyze the [Road Safety and Traffic Demographics dataset (UK)](https://www.kaggle.com/tsiaras/uk-road-safety-accidents-and-vehicles), containing accidents reported by the police between the years of 2004 - 2017. 

### PROJECT GOALS:
* identify factors responsible for most of the reported accidents.
* Build a machine learning model that is capable of accurately predicting the severity of an accident.
* Provide recommendations to the Department of Transport (UK Government), to improve road safety policies and prevent recurrences of severe accidents where possible.

### PACKAGES USED:
* Scikit-learn, numpy, pandas, imblearn (imbalanced-learn), seaborn, Matplotlib

### MOTIVATION
World Health Organization (WHO) reported that more than 1.25 million people die each year while 50 million are injured as a result of road accidents worldwide. Road accidents are the 10th leading cause of death globally. On current trends, road traffic accidents are to become the 7th leading cause of death by 2030 making it a major public health concern. Between the years 2005 and 2016, there were roughly 2 million road accidents reported in the United Kingdom (UK) alone of which 16,000 were fatal.

As a big data project, I wanted to explore the traffic demographics data in greater detail using machine learning! 

### CONTEXT
The UK government amassed traffic data from 2004 to 2017, recording over 2 million accidents in the process and making this one of the most comprehensive traffic data sets out there. It's a huge picture of a country undergoing change.

Note that all the contained accident data comes from police reports, so this data does not include minor incidents.

*For steps undertaken to pre-process and clean the data, please view the "Data Cleansing & Descriptive Analysis_UK Traffic Demographics.ipynb" file*

## DESCRIPTIVE ANALYTICS (EDA)

* Tools used include Python, Tableau, MS PowerBI

### Percent (%) distribution of target classes

![Percent dist of Accident Severity](https://user-images.githubusercontent.com/54816432/64552229-d21da980-d304-11e9-95ef-57588e9379cd.png)

*As seen above, the data is highly imbalanced. This was dealt with using several techniques including resampling, using different performance metrics, using Decision Tree based algorithms, etc. Please refer to the python file for more details.*

For detailed steps undertaken to deal with the imbalanced data, please view the "Modelling_Predictive Analytics_UK Traffic Demographics.ipynb" file.

[This article](https://towardsdatascience.com/metrics-for-imbalanced-classification-41c71549bbb5) provides some great tips on utilizing the correct performance metrics when analyzing a models performance trained on an imbalanced dataset.

[This article](https://machinelearningmastery.com/tactics-to-combat-imbalanced-classes-in-your-machine-learning-dataset/) describes several strategies that can help combat the case of a severly imbalanced dataset. Methods include: 
* Resampling strategies (under - Tomek Links, Cluster Centroids, over sampling - SMOTE)
* Using Decision Tree based models
* Using Cost-Sensitive training (Penalize algorithms)

### Number of accidents by Year and Accident Severity

![Total accidents by year and severity](https://user-images.githubusercontent.com/54816432/64552609-96cfaa80-d305-11e9-8ad6-f01d0d7be5d2.png)

*It can be seen above that the trend seems to be increasing as the years go. In addition, the spike between 2008 - 2009 was because of a enhancement in the reporting system introduced in the UK in 2009, where all accident including minor accidents needed to be reported by the police so as to match the counts represented by hospitals, insurance claims etc.* 

### Accidents density by Location

![geomap](https://user-images.githubusercontent.com/54816432/64553068-ab607280-d306-11e9-8079-985605c98287.png)

*Most accidents took place in major cities - Birmingham, London, leeds, Newcastle

### Accidents by Gender and Age

![Accidents by gender and age](https://user-images.githubusercontent.com/54816432/64553224-fda19380-d306-11e9-836c-81fa478778e6.png)

### Accidents by Day of the week and Year

![Accidents by year and weekday](https://user-images.githubusercontent.com/54816432/64553442-5bce7680-d307-11e9-8c3a-4fdc206acec1.png)

*Most accidents take place on a Friday*

### Vehicle Manoever at time of accident

![Vehicle Manoever at time of accident](https://user-images.githubusercontent.com/54816432/64554775-0e9fd400-d30a-11e9-8a69-f2bc5336cee9.png)

*Most accidetns take place as a result of overtaking*

#### For more findings, please go to the "Images" folder.

#### For steps undertaken to carry out some predictive modeling and hyper-parameter tuning, please view the "Modelling_Predictive Analytics_UK Traffic Demographics.ipynb" file.

## RECOMMENDATIONS TO THE DEPARTMENT OF TRANSPORT (UK)

* Decrease emergency response times during afternoon rush-hours (15-19) especially on Fridays.
* Allocate resources to investigate high density traffic points and identify new infrastructure needs to divert traffic from dual-carriage ways.
* Explore conditions of vehicles and casualties such as vehicle type, age of vehicles registered, pedestrian movements, etc. for policy makers.
* Adopt comprehensive distracted driving laws that increase penalties for drivers who commit traffic violations like aggressive overtaking.

# Acknowledgements
The license for this dataset is the Open Givernment Licence used by all data on data.gov.uk. The raw datasets are available from the UK Department of Transport website.

### I had a lot of fun working on this dataset and learned a lot in the process. I plan to further my research in the area of predictive modeling using imabalanced data and how to effectively build a highly robust model for future projects.
