# Berlin Marathon Data Analysis

In this project I utilised data analysis methods using python to compare data from the 2009 and 2017 Berlin Marathons. Both datasets contain over 35,000 entries.
The aim of this project was to identify any evidence of advancements in marathon preparation, pacing strategies, training technology etc., visible in the comparison of the results. 

## Python Libraries Utilised
- pandas
- seaborn
- matplotlib
- numpy

## Approach / Data Preparation 
I translated the german column headings to english to allow for more coherent analysis.

Entries featuring columns with missing data were removed (approximately 55 entries)
There were some signs of data entry errors as a supposed 108 year old competed in the 2009 Berlin Marathon according to the dataset. This entry was also removed.

## Data Augmentation
The following columns were created from existing columns
- Age (marathon year - birthyear column)
- net (time)
- net_seconds (time in seconds)
- net_minutes (time in minutes)
- half_marathon (half marathon time)
- halfm_seconds (half marathon time in seconds)
- halfm_minutes (half marathon time in minutes)
- pacing (total time - half marathon time)
- split (denotes a positive/even/neutral split of each runner)

## Data Analysis
The following analysis was performed on the 2009 Berlin Marathon data and validated on the 2017 Berlin marathon data.
- Data Characterisation
- Gender breakdown of competitors
- Distribution of finishing times between genders
- Relationship between half marathon time and overall marathon completion time
- Pacing and split impact analysis
- Split analysis (mean finishing times, distribution of splits,...)
- Split data broken down by age categories
- Relationship between age and split times
- 'Bonking' analysis (Note: A competitor is considered to have 'bonked' if the second half of their marathon took 30% longer than their first half.
- Breakdown of bonking data by age, gender

## Notable Findings
- Considerable decrease in proportion of 'bonking' in 2017 when compared to 2009
- Similar decrease in proportional occurance of positive splits in 2017 compared to 2009
      > Male 2017: 78.3% positive splits | Male 2009: 87.6% positive splits
      > Female 2017: 76.5% positive splits | Female 2009: 85.6% positive splits
- Increase in number of even splits in 2017 when comared to 2009
- Increase in percentage of female competitors in 2017 compared to 2009
- Age had a very minimal correlation with pacing for both marathons
- The performance of age groups 18-20, 21-30, 31-35 improved and reduced the gap to the 36-40 age group from 2009 to 2017

## Conclusions
After performing my analysis I can conclude that there is a clear improvement in the performance of athletes from the 2009 Berlin Marathon to the 2017 Berlin Marathon. This improvement could be due to advancements in training technologies or advancements in health and fitness sciences in the years between both marathons. 
