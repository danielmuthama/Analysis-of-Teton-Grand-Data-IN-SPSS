### Analysis-of-Teton-Grand-Data-IN-SPSS



					Visualizing, Analyzing and Explaining Teton Grand Data
								Outline
									
1.	Create a comprehensive explanation of ways in which Teton Grand may be able to use probability statistics and sample concepts when analysing their data. 
2.	Be sure to define the concepts and use examples to highlight what they mean and how they might be relevant for Teton Grand. 
3.	Please be sure that you are posting in a client-ready format, using professional and appropriate language for talking to an organization.

						Analysis of Teton Grand data
								Introduction
In sampling a population or universe is defined as all items in an inquiry field while census inquiry is defined as a complete enumeration of all items in a population.
								 Definition of terms
		• Sampling error – 
	
This is a random variation in a sample estimate from the actual population parameters. Sampling error occurs equally and randomly – their nature can be of compensatory type and the expected value of such errors happens to be equal to zero. It can only be measured for a given sample design and size.

		• Measure of reliability – 
	
This is the steadiness of different measurement of the same thing

		• Standard error – 
	
Standard error’s sample provides a quite accurate representation of a certain population, although sometimes it may produce means which are completely out of distribution tail – relatively far from the main mean. Therefore, standard error known for providing a definite method for measuring and defining sampling – it measures the standard average between the population mean and the sample mean (Tian et al., 2007).

		• Probability sampling –
	
It is also referred to as chance sampling or random sampling. Random sampling has equal chances of inclusion. The gathered results from the probability or random sampling can be expressed in terms of probability – therefore it be very easy to estimate and measure significance or errors of the obtained results which bring about superiority in random sampling (Mardia, 2013).

		• Probability and distribution of a sampled mean

Teton Grand variable definition

    1.	Item 1(i1) - The course helped me advance my understanding of animal health and welfare
    2.	Item 2(i2) - The people I was in class with cooperated to uphold Teton Grand's mission
    3.	Item 3(i3) - The course helped me advance my understanding of environmental health and welfare
    4.	Item 4(i4) - Environmental preservation is one of Teton Grand's top priorities
    5.	Item 5(i5) - The instructors here are committed to a strong, effective education program
    6.	Item 6(i6) - I believe that what I am doing in my immersion course is important for the preservation of The Great Outdoors
    7.	Item 7(i7) - I understand the organization's mission statement and philosophy
    8.	Item 8(i8) - My instructor was effective in teaching the course material
    9.	Item 9(i9) - My instructor wanted me to have a good experience in the course
    10.	Item 10(i10) - I am enthusiastically committed to achieving our organization's objectives
    11.	Item 11(i11) - The rooms used for the training course were conducive to my learning
    12.	Item 12(i12) - The books used for the training course were conducive to my learning
    13.	Item 13(i13) - The immersion activities (i.e., animal learning excursions, park clean-ups) were conducive to my learning
    14.	Item 14(i14) - This organization is effective in implementing environmental change.
    15.	Item 15(i15) - I got regular feedback on how I was performing in the course
    16.	Item 16(i16) - I have been adequately trained to handle the different aspects of environmental preservation
    17.	Item 17(i17) - My instructor was timely and attentive
    18.	Item 18(i18) - My instructor showed a mastery of the course material.
    19.	Item 19(i19) - The course has advanced my appreciation of animal and environmental health and welfare
    20.	Item 20(i20) - This course gave me a sense of accomplishment
    21.	B4(1) – Monday
    22.	B4 (2) – Saturday 










PART A

1.	Monday 
 
a)	Frequency 
  

 
 
 
 

 

 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
  
  


 
 

 
 
 
 

 
 
b)	Saturday 

		    FREQUENCIES VARIABLES=i1 i2 i3 i4 i5 i6 i7 i8 i9 i10 i11 i12 i13 i14 i15 i16 i17 i18 i19 i20
		      /HISTOGRAM NORMAL
		      /ORDER=ANALYSIS.

Frequency distribution
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
 
PART B

1)	Z-SCORE PROPERTY VISUALIZATION AND ANALYSIS


1.	Monday

a)	Descriptive


		     DESCRIPTIVES VARIABLES=Zfinalscore
		      /SAVE
		      /STATISTICS=MEAN STDDEV VARIANCE RANGE SEMEAN 
		     KURTOSIS SKEWNESS.



 



b)	Frequencies



		     FREQUENCIES VARIABLES=Zfinalscore
		      /ORDER=ANALYSIS.



 
 

 
2.	Saturday 



a)	Descriptive 


		    DESCRIPTIVES VARIABLES=Zfinalscore
		      /SAVE
		    /STATISTICS=MEAN STDDEV VARIANCE RANGE SEMEAN KURTOSIS SKEWNESS.




 




b)	Frequency 


		    DATASET ACTIVATE DataSet3.
		    FREQUENCIES VARIABLES=Zfinalscore
		    /HISTOGRAM NORMAL
		    /ORDER=ANALYSIS.





 

 

 





3.	Monday and Saturday



1.	Descriptive 

	    DESCRIPTIVES VARIABLES=Zfinalscore
	      /SAVE
	      /STATISTICS=MEAN STDDEV VARIANCE RANGE SEMEAN KURTOSIS SKEWNESS.


 


2.	Frequency 

	    FREQUENCIES VARIABLES=Zfinalscore
	      /HISTOGRAM NORMAL
	      /ORDER=ANALYSIS.


 

 




2)	TEST FOR NORMALITY


1.	Saturday 


	    EXAMINE VARIABLES=Zfinalscore
	      /PLOT BOXPLOT STEMLEAF HISTOGRAM NPPLOT
	      /COMPARE GROUPS
	      /STATISTICS DESCRIPTIVES
	      /CINTERVAL 95
	      /MISSING LISTWISE
	      /NOTOTAL.




 

 


 


 
  



 
 




2.	Monday 



* Define Variable Properties.
	
	




 


 


 

 
 



 
 



3.	Monday and Saturday



	    EXAMINE VARIABLES=Zfinalscore
	      /PLOT BOXPLOT STEMLEAF HISTOGRAM NPPLOT
	      /COMPARE GROUPS
	      /STATISTICS DESCRIPTIVES
	      /CINTERVAL 95
	      /MISSING LISTWISE
	      /NOTOTAL.




 

 


 



 


 



 
 

			Explanation

		Percentage confidence of the event happening
				 Monday 
		    1.	Item 1(i1) – 97.3
		    2.	Item 2(i2) – 96.2
		    3.	Item 3(i3) – 97.8
		    4.	Item 4(i4) – 97.8
		    5.	Item 5(i5) – 98.9
		    6.	Item 6(i6) – 98.4
		    7.	Item 7(i7) – 97.3
		    8.	Item 8(i8) – 98.4
		    9.	Item 9(i9) – 98.4
		    10.	Item 10(i10) – 97.8
		    11.	Item 11(i11) – 98.4
		    12.	Item 12(i12) – 97.8
		    13.	Item 13(i13) – 98.4
		    14.	Item 14(i14) – 97.8
		    15.	Item 15(i15) – 97.8
		    16.	Item 16(i16) – 98.9
		    17.	Item 17(i17) – 96.8
		    18.	Item 18(i18) – 96.2
		    19.	Item 19(i19) – 97.3
		    20.	Item 20(i20) - 97.3

		Saturday

		    1.	Item 1(i1) – 100
		    2.	Item 2(i2) – 99.7
		    3.	Item 3(i3) – 99.4
		    4.	Item 4(i4) – 99.7
		    5.	Item 5(i5) – 99.7
		    6.	Item 6(i6) – 99.7
		    7.	Item 7(i7) – 99.7
		    8.	Item 8(i8) – 100
		    9.	Item 9(i9) – 100
		    10.	Item 10(i10) – 99.4
		    11.	Item 11(i11) – 99.7
		    12.	Item 12(i12) – 100
		    13.	Item 13(i13) – 99.7
		    14.	Item 14(i14) – 100
		    15.	Item 15(i15) – 99.7
		    16.	Item 16(i16) – 100
		    17.	Item 17(i17) – 99.7
		    18.	Item 18(i18) – 99.7
		    19.	Item 19(i19) – 99,4
		    20.	Item 20(i20) – 99.4
	
					Z-Analysis

	1.	Monday and Saturday

			    Kurtosis: - has std error of 0.218, statistic of 10.959
			    Skewness: has std error of 0.109, statistic of -2.417
			    Mean: std error of 0.04467671

	2.	Monday 

			    Kurtosis: has std error of 0.273, statistic of 10.577
			    Skewness: has std error of 0.137, statistic of – 2.570
			    Mean: std error of 0.05625440

	3.	Saturday

			    Kurtosis: has std error of 0.07352146, statistic of 10.959
			    Skewness: has std error of 0.179, statistic of -2.570
			    Mean: std error of 0.07352146

			Testing for normality – true if (std error of the mean >= 0.05)
			
			    1.	Monday and Saturday: has a std error of 0.04467671
			    2.	Monday: has a std error of 0.07352146
			    3.	Saturday: has a std error of 0.05625440
 
								References
	    
Mardia, K. V. (2013). Applications of some measures of multivariate skewness and kurtosis in testing normality and robustness studies. Sankhyā: The Indian Journal of Statistics, Series B, 115-128.
Tian, L., Cai, T., Goetghebeur, E., & Wei, L. J. (2007). Model evaluation based on the sampling distribution of estimated absolute prediction error. Biometrika, 94(2), 297-311.

