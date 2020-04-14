# data_repository_yang
NO2 exposure and its health effect data sets.

## Summary

This repository was prepared for the final project of Environmental Data Analytics (ENV 872L) at Duke University, Spring 2020. It includes one folder with four data sets. The goal is to analyze the association between exposure to NO2 and the level of two urinary biomarkers, 8-isoprostane, 11-dehydrothromboxane B2 (11dhTxB2)


## Investigators
The investigator is Yang Wang, who is a master student at Duke University. The contact email is yangwangbluedevil@gmail.com. 

## Keywords

NO2, air pollutants, exposure to NO2, health effect, 8-isoprostane, 11-dehydrothromboxane B2 (11dhTxB2)

## Database Information
All the data are from Jim Zhang's lab. Jim Zhang is a professor at the Nicholas School of Environment at Duke University


## Folder structure, file formats, and naming conventions 
This data repository only includes one folder called "the data for the final project". This folder includes four data sets and they are all in the format of excel.csv files. The file 8-iso is the data set of urinary biomarker 8-isoprostane. The file 11-dh is the data set of urinary biomarker 11-dehydrothromboxane B2 (11dhTxB2). The file urine_info is the data set that has information about the subjects who provided the urine samples. The urine list is a data set with lists of information of sample ID, subject ID and visits.


## Metadata
The meaning of the columns as well as units and class of the data in each foler is listed belowe. Column names without descriptors are irrelevant to this study.

For data set "Urine List					
No.	Column	Column Name	 Meaning	                           units	    class of the data
1	    1	    Sample ID	   the identity number of the samples	  NA	       integer
2	    2	    Subject ID	 the identity number of the subjects	NA	       integer
3	    3	    visit	the    number of the 4 visits (1,2,3 or 4)	NA	       integer

8-iso & 11-dh				
No.	Column	Column Name	    Meaning                        	            Units	      Class of the data
1	   2	    Sample ID       the identity number of the samples	         NA	        integer
2	   5	    Calculated Conc	the concentration tested by the machine      ng/ml	    numeric
3	   6	    Sample Conc	    the concentration in the original urine	     ng/ml	    numeric

Urine Info					
No.	Column	Column name	  Meaning	                                Units	 Class of the data
1   1	      Sample_ID	    the identity number of the samples    	NA	    integer
2	  2	      Subject ID	  the identity number of the subjects   	NA	    integer
3	  4	      visit	        the number of the 4 visits (1,2,3 or 4)	NA	    integer
4	  5	      group	        group, A or B	NA	category
5	  6	      COLD	        cold ( represent respiratory infection)	NA	    category
6	  7	      MNST	        menstruation                           	NA	    category
7	  8	      last.ate    	the hours to the last meal	            hours	  integer
8	  9	      wkday.start 	the day that the subject start their work	NA  	category
9	  21	   dt_smoke	      second-hand smoke exposure in hours	    hours	  numeric
10	22	    USG	urine     specific gravity	                      g/ml	  numeric
11	31    	o3exp.12h	    the exposure of ozone in 12h	          ug/m3	  numeric
12	32    	pmexp.12h	    the exposure of PM2.5 in 12h	          ug/m3	  numeric
13	33	    no2exp.12h  	the exposure of NO2 in 12h	            ug/m3	  numeric
14	34    	so2exp.12h  	the exposure of SO2 in 12h	            ug/m3	  numeric
15	35	    Temp.12h    	average temperature in 12h              ug/m3	  numeric
16	36	    RHx.12h	      average humidity in 12h	                ug/m3	  numeric
17	41    	o3exp.24h   	the exposure of ozone in 24h           	ug/m3	  numeric
18	42    	pmexp.24h   	the exposure of PM2.5 in 24h	          ug/m3	  numeric
19	43    	no2exp.24h	  the exposure of NO2 in 24h	            ug/m3 	numeric
20	44    	so2exp.24h	  the exposure of SO2 in 24h	            ug/m3 	numeric
21	45    	Temp.24h	    average temperature in 24h	            ug/m3 	numeric
22	46    	RHx.24h	      average humidity in 24h	                ug/m3	  numeric
23	51    	o3exp.1w	    the exposure of ozone in one week	      ug/m3   numeric
24	52	    pmexp.1w	    the exposure of PM2.5 in one week	      ug/m3	  numeric
25	53    	no2exp.1w	    the exposure of NO2 in one week	        ug/m3 	numeric
26	54    	so2exp.1w	    the exposure of SO2 in one week       	ug/m3	  numeric
27	55    	Temp.1w	      average temperature in one week	        ug/m3	  numeric
28	56	    RHx.1w	      average humidity in one week	          ug/m3	  numeric
29	61    	o3exp.2w	    the exposure of ozone in two weeks	    ug/m3	  numeric
30	62    	pmexp.2w	    the exposure of PM2.5 in two weeks	    ug/m3	  numeric
31	63    	no2exp.2w	    the exposure of NO2 in two weeks	      ug/m3	  numeric
32	64    	so2exp.2w	    the exposure of SO2 in two weeks	      ug/m3	  numeric
33	65    	Temp.2w	      average temperature in two weeks	      ug/m3	  numeric
34	66	    RHx.2w	      average humidity in two weeks	          ug/m3 	numeric


## Scripts and code
No scripts and codes.

## Quality assurance/quality control

The limit of detection for 8-isoprostane was 0.016ng/ml. The minimum detection limit for 11-dhTxB2 is 0.065ng/ml. Any value which is below 0.016 in the column of calculated Conc in 8-is data set should be excluded as an error. Any value which is below 0.065 in the column of calculated Conc in 11-dh data set should be excluded as an error.