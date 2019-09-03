# Analyzing_Road_Safety_UK_classification

# Summary
Analyzed the Road Safety and Traffic Demographics dataset (UK), containing accidents reported by the police between the years of 2004 - 2017. The goal was to identify the factors responsible for most of the reported accidents, create a ML model that was capable of accurately predicting the severity of an accident and finally, provide recommendations to the Department of Transport (UK Government), to improve road safety policies and prevent recurrences of severe accidents where possible.

# Context
The UK government amassed traffic data from 2004 to 2017, recording over 2 million accidents in the process and making this one of the most comprehensive traffic data sets out there. It's a huge picture of a country undergoing change.

Note that all the contained accident data comes from police reports, so this data does not include minor incidents.

# Motivation
World Health Organization (WHO) reported that more than 1.25 million people die each year while 50 million are injured as a result of road accidents worldwide. Road accidents are the 10th leading cause of death globally. On current trends, road traffic accidents are to become the 7th leading cause of death by 2030 making it a major public health concern. Between the years 2005 and 2016, there were roughly 2 million road accidents reported in the United Kingdom (UK) alone of which 16,000 were fatal.

As a Big Data project, I wanted to explore the traffic demographics data in detail using machine learning! I tried to build a classifier that could predict the severity of an accident given a set of input factors. In addition, I wanted to display several techniques that I exmployed in order to deal with a severly imbalanced dataset.

# Content
The data comes from the Open Data website of the UK government, where they have been published by the Department of Transport.

The dataset comprises of two csv files:

Accident_Information.csv: every line in the file represents a unique traffic accident (identified by the Accident_Index column), featuring various properties related to the accident as columns. Date range: 2005-2017.

Vehicle_Information.csv: every line in the file represents the involvement of a unique vehicle in a unique traffic accident, featuring various vehicle and passenger properties as columns. Date range: 2004-2016.

The two above-mentioned files/datasets can be linked through the unique traffic accident identifier (Accident_Index column).

# Acknowledgements
The license for this dataset is the Open Givernment Licence used by all data on data.gov.uk. The raw datasets are available from the UK Department of Transport website.
