# Detecting Changes in Ca Fluorescent Activities During Behavioral Events
#######################################################################################################

# Background
Data relating to reaction time and physiological signals are limited by physical constraints.  There is only so fast our muscles groups can move,  or there's so fast a cells sodium-potassium pumps can restore the resting poential of the cell. As a result, those data are not suitable for use with parametric methods that relies on the initial believe of normal distribution.  To test the hypothesis that there were no relationship in Ca activities event rates between baseline and cue period, the Ca event rates for each period were calculated and compared using 10,000 round paired permutations.

#######################################################################################################
# Random Permutation Introduction (example with responses duirng cue period )

1.  For each trial,  event rates between baseline and cue were randomly shuffled (This preserves the shared variances within trials )
2.  The mean event rates for baseline and cue for each shuffeled samples were calculated.
3.  A mean difference distribution were created using each baseline and cue pairs). This is called the "Permutation distribution".
4.  Cout up the percentage of cases that  the values were more extreme than the original sample mean.
5.  If the total percentage of cases < 0.025, the differences is considered significant (alpha adjustment will be needed for multiple comparsions).  
  

![Fig_P_1](https://github.com/user-attachments/assets/d5eb049b-5ec9-4a85-a25c-8d8c20ab9230)
#######################################################################################################


The permutaiton script we put together using this logic is producing the same results as a more commonly use package from mlxtend.  
Our sciprt is attached here for demonstration purpose, but we will be using mlxtend package for performance reason.  

[0_Ka_Tool_Independent_Permutation]
![Fig_P_2](https://github.com/user-attachments/assets/bb11d7e5-4473-464f-90bf-13e5ffee7053)
#######################################################################################################
