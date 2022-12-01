# BMIN503/EPID600 Final Project

Final Project:

Overview: 
This project aims to evaluate blood product transfusion at the Hospital of the University of Pennsylvania.  I will use a dataset from 2021 that includes all transfusions performed, and the patient’s complete blood count, clotting tests, and other parameters. The goal is to assess how often patients received transfusions when they fell outside the established clinical guidelines for blood components.

Introduction:
Blood product transfusion is a common and lifesaving intervention for patients, but despite its benefits, it also introduces risks for patients, including the risk of transfusion reaction, infectious complications, and alloimmunization. Many studies over the past few decades have demonstrated that transfusion thresholds that are more conservative, i.e. more restrictive, lead to better patient outcomes than liberal transfusion thresholds. I am examining an operational dataset which contains blood products administered to patients, and their hematologic lab values, which will be compared to established transfusion guidelines. 

Obviously, there are many complex factors that play into whether a transfusion is indicated, and transfusion thresholds may be personalized for patients, but it will be helpful to describe practices and trends to identify areas for potential intervention. There are several specific questions of particular interest to the blood bank, notably how often clinicians evaluate the corrected count increment after platelet transfusion.  Other concerns include the size of the population with certain transfusion thresholds, and identifying practice patterns for particular providers. In general, knowing how blood products are used allows the blood bank to more accurately predict blood needs in the future, which allows for better planning and inventory management.

Methods: 
* means that this is NOT a de-identified variable, so I need to de-identify it for this project.
KEY means that I think this column will be crucial for analysis.

Columns I have:
*KEY MRN- char
*Patient Name- char
KEY Transfusion_Date- numeric
KEY Product_type- char- may be red blood cells, single donor platelets, pathogen reduced platelets, thawed cryo, thawed plasma, whole blood
Transfused_vol- numeric, standardized, not trustworthy
Order_Name- char – not high yield, because result code is better.
Order_date- numeric- not high yield, because collect is more important
KEY Collect_date- numeric- KEY
Result_date- numeric
*Accession_nbr- char
KEY Result_code- char. Platelets, hbg, INR
KEY Result- numeric
*Order_phys- char



Analysis that should be done:

For each product:
How many patients received transfusions, and how many units did they receive- over what time period?

For those who received platelet transfusions, how many had a platelet count performed beforehand?  After?  What was the distribution of those values?

For those who received red blood cells, how many had a hemoglobin performed beforehand?  After?  What was the distribution of those values?

How many patients received a single unit of FFP? What was their INR?


Were the ordering practices different for different ordering physicians?


How would we predict the need for products given this information?
![image](https://user-images.githubusercontent.com/99358869/205093254-1f09721b-e233-4bd3-ad92-fd3d32eede02.png)


