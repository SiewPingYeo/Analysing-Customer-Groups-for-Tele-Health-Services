# Analysing-Customer-Groups-for-Tele-Health-Services

### Content: 
1.	Problem Statement
2.	Approach:
3.	Analysis Results
a.	User Segment: Members who are in the majority age group of 25 to 45 years old
b.	User Segment: Members who are not covered under insurance
c.	Customised strategies according to the top 10 diagnoses 
d.	Other interesting insights
4.	Additional data required for more insights
5.	Visualisation tool and how it can be maintained 


**1.	Problem Statement:**
-	To identify three user segments/insights for potential targeting strategies 
-	To propose recommendations for each user segment/insight for customised targeting strategies for the marketing team

**2.	Approach:** 
-	In order to get a better understanding of the users of the tele-health app, the exploratory data analysis (codes in the attached jupyter notebook) will start off by looking into the demographics of the members. This will provide a base understanding of the majority user group and the type of members that will potentially use the app. 

-	Subsequently, the EDA will dive deeper into how the demographics interact with the other features given in the dataset. This will provide better insights into the habits or behaviour of the user groups.  From the observations made through these multivariate explorations, gaps and distinct user groups can be identified and customised recommendation strategies can be given for each user group. 

-	Besides customising recommendations for the identified user groups, the recommendations will also take into account of the benefits for the company in terms of consultation revenue. 


**3.	Analysis Results:** 

(a)	User Segment: Members who are in the majority age group of 25 to 45 years old
o	Based on the histogram below, a large majority of the members falls within the age group of 25 to 45 years old.  The minority groups are made up of children, teenagers as well as the elderly. 
 ![histogram](https://user-images.githubusercontent.com/94337686/177003682-a99fd7e1-1d05-4eaf-8df2-ce388e01dc01.png)



(b)	User Segment: Members who are not covered under insurance
o	There are still a sizable proportion of members who are not under insurance coverage and this target group is an important one. 
o	From the boxplots below, those without insurance cover falls between the age group of 25 to 40.  There are also more males who do not have insurance coverage compared to females. 
o	Majority of those insured also falls within the age group of 25 to 40 years old. This could be due to the fact that most come from the working population and have more awareness of the importance of healthcare insurance. They might also be covered under health insurance provided by the company that they are working for. 
  

o	Those with insurance coverage are also more likely to purchase medicine, which could potentially lead to higher consultation revenue. From the left count plot below, there are more insured members purchasing medicine compared to the non-insured members. In addition, the bar plot on the right also shows that the consultation revenue was actually the higher when members purchased prescribed medicine and are under insurance coverage. 

  ![21](https://user-images.githubusercontent.com/94337686/177003756-3c292540-7a28-408a-9354-9850b52f9df2.png)

![22](https://user-images.githubusercontent.com/94337686/177003758-018a3eaf-2d98-4e4e-8f08-831e87f7f715.png)

 
![23](https://user-images.githubusercontent.com/94337686/177003761-6dd5a20a-d7b3-4119-9eeb-61fef878a626.png)

![24](https://user-images.githubusercontent.com/94337686/177003763-7dbe9b44-3f8c-4c88-a2a6-c0feba5af23c.png)

(c)	Customised strategies according to the top 10 diagnoses 
o	From the exploratory data analysis performed, the top 10 most common diagnosis codes are : 
1. Muscle strain
2. Chronic lower back pain
3. Covid-19
4. Complications of immunization
5. Rash and non-specific skin eruption
6. Dysmenorrhea
7. Unsuitable
8. Headache
9. Acute upper respiratory infection
10. Gastroenteritis and colitis

o	From the EDA plots, those above 45 years old tend to have urinary disorders and soft tissue disorders compared to other age groups. 
o	Out of all the top 10 diagnosis codes for all user groups, ‘unsuitability’ is always one of the top 5 codes. 
 
 ![31](https://user-images.githubusercontent.com/94337686/177003785-6cace9dc-3c85-4acb-924a-6d88406cd9a7.png)

 
 
(d)	Other interesting insights: 
o	Although the majority of the users are females, the consult revenue is actually higher for males (almost three times higher). 

![4](https://user-images.githubusercontent.com/94337686/177003805-8827f6e0-0bc7-4239-99d5-6c636502e203.png)
![41](https://user-images.githubusercontent.com/94337686/177003811-b4369a65-8f30-4e72-8523-56468182186a.png)

 
	Consult revenue is also dependent on the type, amount and price of the medicine that was dispensed. The higher consult revenue could be attributed to the price and amount of medicine that was dispensed to the male patients during the months of Oct – Dec 2021. The price and amount of medicine dispensed to the male patients might be much higher compared to the females according to their medical conditions. 
o	Consult revenue is also higher for members who bought medicine and those who chose delivery type 2 and 3; therefore there could be a EDM promotion of these delivery types (convenience) as a selling point of the tele-health service – encouraging members to purchase medicine through delivery type 2 and 3. 
 

**4.	Additional data required:** 

o	It would be great if there are additional data on consultations which are rejected due to its unsuitability for tele-consultations. Currently, unsuitable consultations are only shown through diagnosis codes. As some cases are better addressed through the GP physically, it would also be helpful to identify the symptoms reported by the patients for those unsuccessful consultations. The members can then be better educated through EDMs on the suitability of a tele-consult based on conditions. Lesser rejections can also lead to increase efficiency and consult revenue in the long run.
o	The price and amount of medicines prescribed would also allow better exploration on the relationship between consult revenue and gender and explain the interesting insight on how male patients could generate higher consult revenue than females despite the high number of female patients in the months of Oct to Dec 2021. 

**5.	Visualisation Tool and how it can be maintained:** 

o	The visualisation tool, Tableau, can be used to provide an overview of the trends, thus influencing business decisions. 
o	The screenshot below shows a sample of a dashboard created in Tableau. The Tableau workbook can be found in the folder as well. It allows the user to have a comprehensive summary of the members’ demographics and related profiles, facilitating the creation of customised marketing strategies for different user segments. There are also filters for time period, gender and age groups for the users to zoom into the user segments they would like to visualise. 
o	The visualisation plots shown in the Tableau dashboard can also support the recommendation strategies proposed under the analysis results. 

![tableau](https://user-images.githubusercontent.com/94337686/177003675-e4ce14f3-c38c-4791-a70e-45f0ac3238a8.jpg)

 
o	To ensure that the data source is always updated, it has to be connected to a database such as AWS Redshift, Lambda or Athena, GCP Big Query or any SQL database. This ensures that big data involved can be handled seamlessly and projected on Tableau dashboard.  It can also be created as a real-time dashboard to reflect the current situation accurately and facilitate efficient service recovery or business decisions. 
