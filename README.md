# Diet-Index-HEI
R code for calculating HEI-2015 from NDSR files 4 and 9
The data frame is created by importanting an excel file that contains file 4 and file 9 from each participant.  One diet recall for participant, one row per participant.
The data frame is called df49 (indicating the NDSR files)
Code derived from modifying SAS code for calculating HEI-2015 and code for previous HEI R package. https://github.com/timfolsom/hei/blob/master/R/hei.R

In the data source (excel or csv) prior to importing, recode the following: 
	Participant ID as “cpartid”
	Date of Intake as “dintake” 
	Whole Grains (ounce equivalents) as “WholeGrains_oz”
	Refined Grains (ounce equivalents) as “RefinedGrains_oz”
	Sodium (mg) as “Sodium_mg”
	Total Saturated Fatty Acids (SFA) (g) as “SFA”
	Total Monounsaturated Fatty Acids (MUFA) (g) as “MFA”
	Total Polyunsaturated Fatty Acids (PUFA) (g) as “PFA”
	Added Sugars (by Total Sugars) (g) as “AddedSugars_TotalSugars_g”
	% Calories from SFA as “ripctSFA"
	Energy (kcal) as “kcal”
