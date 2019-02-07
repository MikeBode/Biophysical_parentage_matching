# Biophysical_parentage_matching

The MAT file Input_data_Matlab.mat contains the connectivity matrices produced by the three biophysical models, and the observed connectivity matrix produced by the genetic parentage assignments.

--- AllOutlineWithNumber           
A three column matrix where each row gives a point on the outer polygon of a reef in the Great Barrier Reef. The first column gives the longitude, the second column gives the latitude, the final column identifies the reef number (consistent throughout these data). There are 609 reefs in the wider study region. Note that we have excluded reefs north of 18 S, which we consider too far away to be demographically relevant.

--- Distance                         
A 609x609 matrix containing the Euclidean distance between all the reefs, measured in degrees. 

--- High_density_reefs               
A logical 609x1 vector indicating which reefs are considered “high density”, with a larval output proportional to their reef area. These are the inshore reefs in the study area.

--- Medium_density_reefs             
A logical 609x1 vector indicating which reefs are considered “high density”, with a larval output proportional to their reef area, at 50% of the high density reefs. These midshelf reefs (there are only two of them) are known to contain an approximately equivalent number of both Plectropomus leopardus and P. maculatus.

--- Low_density_reefs                
A logical 609x1 vector indicating which reefs are considered “high density”, with a larval output proportional to their reef area, at 5% of the high density reefs. These offshore and midshelf reefs are dominated by P. leopardus. 

--- MN_pop_mac                       
A 609x1 vector reporting the estimated mean population size of P. maculatus on all of the reefs in the study region.

--- SE_pop_mac                       
A 609x1 vector reporting the standard error in the estimated population size of P. maculatus on all of the reefs in the study region.

--- Num_reefs                        
Number of reefs in the study region (609).

--- Obs_matrix_Cohort_1 & Obs_matrix_Cohort_2              
Connectivity matrix for the genetic parentage assignment dataset. A 610x609 matrix indicating the number of juveniles on the column reef that were assigned to parents on the row reef. The final row contains unassigned juveniles. Values are given for both cohorts of juveniles.

--- PropMPA 
A 1x609 vector indicating the proportion of each reef that is a no-take marine reserve. Most values are 0 or 1, reflecting the fact that marine reserves in the Great Barrier Reef Marine Park contain the entirety of a patch reef.

--- Weighted_Sim_matrix_Cohort_C_XX
Connectivity matrix for the biophysical model simulations. A 609x609 matrix indicating the probability that a larvae released from the row reef survives and dispersers to settle on the column reef. The value of “C” in the variable name indicates the first (1) or second (2) cohort. The value of “XX” indicates the behavioural variant of the biophysical model: consistent (“pp”), varying (“r”), or passive (“n”). 

--- centroid                         
A 609x2 matrix indicating the longitude (first column) and latitude (second column) of every reef in the study region.

--- reef_size_arclength              
A 609x1 matrix indicating the size of each reef in the study region, as measured by the amount of crest habitat (i.e., the length of the reef perimeter). 

