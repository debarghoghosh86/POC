# Overview

In the current scoring process, ‘Critical Error’, ‘Error’ and ‘Warning’ are being used to calculate individual scores for an analysis run. In certain situations the ‘Info’ clusters present in canary/baseline or both will convey significant details to a user. Hence it becomes a necessity to include ‘Info’ cluster data into the regular scoring process.

To overcome this problem the ‘Info’ cluster is introduced into the scoring algorithm. A dedicated colour ‘Blue’ is used to mark the clusters which adds value to the scoring. Not all the ‘Info’ clusters contribute to the scoring and therefore ‘Info’ clusters marked as ‘Blue’ and having score reduction of any type greater than zero will be displayed in the ‘Unexpected’ tab. The remaining ‘Info’ clusters will be displayed in the ‘Ignored’ tab under ‘Ignore’ type.


# Set info-cluster scoring

To set the info-cluster scoring on follow the steps given below:



1. While creating the Log template turn the toggle button on under Log Provider tab as shown below:

   ![alt_text](images/image1.png "image_tooltip")


2. After enabling the INFO scoring feature, a new ‘Info’ field is added under the  ‘Characterization Topic’ drop down in the ‘Log Topic’ tab as shown below:

![alt_text](images/image2.png "image_tooltip")


3. After a run is completed with INFO scoring feature on, UI shall display the ‘Info’ cluster having score reduction greater than zero in the unexpected tab. 

You can reclassify any other topic as ‘Info’ and vice-versa. The same logic shall be applicable to reclassification flow as well as a new run for the same application. The dropdown options in the unexpected and ignored tab should display ‘Info’ field if the INFO scoring feature is turned on. 
 

![alt_text](images/image3.png "image_tooltip")



Note: After selecting the INFO scoring option, it will become a non-editable field while editing the template. This is to maintain the consistency for all the runs under a single application.
