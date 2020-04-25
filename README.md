# data_repository_yang
NO2 exposure and its health effect data sets.

## Summary

This repository was prepared for the final project of Environmental Data Analytics (ENV 872L) at Duke University, Spring 2020. It includes one folder with four data sets. The goal is to analyze the association between exposure to NO2 and the level of  urinary biomarkers 8-isoprostane


## Investigators
The investigator is Yang Wang, who is a master student at Duke University. The contact email is yangwangbluedevil@gmail.com. 

## Keywords

NO2, air pollutants, exposure to NO2, health effect, 8-isoprostane

## Database Information
All the data are from Jim Zhang's lab. Jim Zhang is a professor at the Nicholas School of Environment at Duke University


## Folder structure, file formats, and naming conventions 
This data repository only includes one folder called "the data for the final project". This folder includes three raw data sets and they are all in the format of excel.csv files. The file 8-iso is the data set of urinary biomarker 8-isoprostane.  The file urine_info is the data set that has information about the subjects who provided the urine samples. The urine list is a data set with lists of information of sample ID, subject ID and visits.


## Metadata
The meaning of the columns as well as units and class of the data in each foler is listed belowe. Column names without descriptors are irrelevant to this study.

For data set "Urine List					
Column Name	| Meaning	                            |units |	  class of the data
------------|-------------------------------------|----- |---------------------
 Sample ID	|   the identity number of the samples	  |NA	 |      integer
Subject ID |	 the identity number of the subjects	|NA	    |   integer
 visit	  |   the number of the 4 visits (1,2,3 or 4)	|NA	  |     integer
 
8-iso 			
Column Name	|    Meaning                                   |    Units	  |    Class of the data
------------|----------------------------------------------|------------|---------------------
  Sample ID |      the identity number of the samples	|         NA	   |     integer
 Calculated Conc|	the concentration tested by the machine   |   ng/ml	 |   numeric
Sample Conc	 |   the concentration in the original urine|	     ng/ml	  |  numeric

Urine Info					
Column name|	Meaning                             |	Units|	Class of the data
---------- |--------------------------------------|----- |---------------------
ample_ID  |	the identity number of the samples  |	NA |	integer            
SubjectID  |	the identity number of the subjects| NA	|integer    
COLD	|cold ( represent respiratory infection)|	NA|	category
MNST	|menstration during visit|	NA|	category
last.ate|	the hours to the last meal|	hours	|integer
wkday.start|	the day that the subject start their work	|NA	|category
dt_smoke|	second-hand smoke exposure in hours|	hours	|numeric
USG	urine |specific gravity	|g/ml	|numeric
o3exp.12h|	the exposure of ozone in 12h|	ug/m3	|numeric
pmexp.12h	|the exposure of PM2.5 in 12h|	ug/m3|	numeric
no2exp.12h|	the exposure of NO2 in 12h|	ug/m3	|numeric
so2exp.12h|	the exposure of SO2 in 12h	|ug/m3|	numeric
Temp.12h|	temperature in 12h|	ug/m3	|numeric
RHx.12h|	humidity in 12h	|ug/m3|	numeric

## Scripts and code
No scripts and codes.

## Quality assurance/quality control

The limit of detection for 8-isoprostane was 0.016ng/ml. Any value which is below 0.016 in the column of calculated Conc in 8-is data set should be excluded as an error. 