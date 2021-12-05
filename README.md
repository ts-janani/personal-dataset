# 1990-2021 US School Shootings - Personal Dataset
## Motivation:
I wanted to answer various questions regarding school shootings across the United States, including what type of school is most susceptible, which state they occur in the most, and how many there have been overall. 

## **Data Process:** 
I found the source data at https://www.kaggle.com/ecodan/school-shootings-us-1990present. The original dataset included the date, city, state, area type (urban, suburban, rural), the type of school, the number of fatalities, number of wounded, where the details of each incident was sourced (Wikipedia or the Pah/Amaral/Hagan research), and a short description of the incident. Firstly I cleaned the data, getting rid of the descriptions, area type as well as the wounded. These columns were only about half filled, so I felt they would not produce any solid overall data. I then deleted all the duplicate incidents, by idenitifying duplicate dates in Excel. Some of the data points had the school type missing, so I filled them in with "Unknown". The rest of data was well recorded with no typos, so this left me with my final dataset. 

## **Visualization:**
I created a few visualizations to represent different aspects of the data. 

The first graph depicts the total number of fatalities from school shooting each year. 2012 and 2018 are tied for the most, with 1993 and 2007 closely behind. The second plot shows the cumulative sum of fatalities over the years.

![image](https://user-images.githubusercontent.com/91508008/144691483-0eae6159-760a-417b-bcfd-e3f123bcc4fd.png)
![image](https://user-images.githubusercontent.com/91508008/144728614-216f4de9-c273-4938-a651-b06510dc5dda.png)

This next plot shows the total fatalities by state, from 1990-2021. California takes the leas by quite a large margin, followed by Texas, Florida, Virginia and West Virginia. It is expected that California and Texas are top two considering how they are the most populous states, but Virginia and West Virginia do not fit with that explanation. Further research could be done to understand why they fall in the top 5.

![image](https://user-images.githubusercontent.com/91508008/144691560-c786fb4f-5bbd-428b-bf4f-82229dc34a1c.png)

The fourth plot depicts the frequency of school shootings sorted by type of school - College, High School, Middle School, Elementary, and Unknown. High School outranks the others by a large margin. 

![image](https://user-images.githubusercontent.com/91508008/144729091-ac62fdbf-e9f1-4db0-92f4-9ed0f2e95a46.png)

The last plot shows the frequency of fatalities from each incident. Most incidents end with just zero or one fatality, and the incident with the most fatalities had over 30. 

![image](https://user-images.githubusercontent.com/91508008/144729125-3dc6006c-a28b-4c59-b23f-f5d1e911de5d.png)

## **Analysis:** 
I found Tukey's five number summary of the fatality frequency using the summary function in R. Using IQR, I found that anything over 1 fatality in an incident is an outlier. Here is the boxplot representation of the five number summary.

![image](https://user-images.githubusercontent.com/91508008/144729900-1a9f4e0c-8600-4b5b-b45e-a9495312ce07.png)

![image](https://user-images.githubusercontent.com/91508008/144729878-c2227608-0f13-468a-b7b2-9fd4df55ea23.png)













