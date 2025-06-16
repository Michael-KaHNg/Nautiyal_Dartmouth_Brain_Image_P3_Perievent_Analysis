# Detecting Changes in Ca Fluorescent Activities During Behavioral Events

# Background
Data relating to reaction time and physiological signals are limited by physical constraints.  There is only so fast our muscles groups can move,  or there's so fast a cells sodium-potassium pumps can restore the resting poential of the cell. As a result, those data are not suitable for use with parametric methods that relies on the initial believe of normal distribution.  To investigate how does Ca activities changes during the behavioral task,  the Ca event rates during different time periods of a task were calculated and compared against a pre-trial baseline period using Paired 10,000 round permutations.

# Random Permutation Introduction (example with responses duirng cue period )

1.  For each trial,  event rates between baseline and cue were randomly shuffled (This preserves the shared variances within trials )
2.  The mean event rates for baseline and cue for each shuffeled samples were calculated.
3.  A mean difference distribution were created using each baseline and cue pairs). This is called the "Permutation distribution".
4.  Cout up the percentage of cases that  the values were more extreme than the original sample mean.
5.  If the total percentage of cases > 0.025, the differences is considered significant (alpha adjustment will be needed for multiple comparsions).  
  

![Fig_P_1](https://github.com/user-attachments/assets/d5eb049b-5ec9-4a85-a25c-8d8c20ab9230)

![Fig_P_2](https://github.com/user-attachments/assets/bb11d7e5-4473-464f-90bf-13e5ffee7053)
