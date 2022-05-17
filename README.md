# Kickstarting with Excel

## Overview of Project
This project is carried out at the request of our client, Louise, who is considering launching Kikstarter campaign with a funding goal of 

!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

 to support her play “Fever”. The analysis is performed to determine if there are any specific factors related to the success of croudfunding campaigns in theater category on Kickstarter. The source, for the analysis, is the data set of Kickstarter campaigns (over 4000 campaigns) for the period from 2009 till 2017, which is condensed, sorted and visualized through Pivot Tables and Pivot Charts on MS Excel.
### Purpose
The purpose of the analysis is to provide the client with the greater understanding of how different campaigns fared in relation their launch dates and their funding goals, so that she could set her campaign to mirror other successful campaigns in the same category.
## Analysis and Challenges
Before getting to the analysis, let’s see what formulas were implemented to the dataset, Kickstarter_Challenge.xle and major changes were made. 
-	Two columns (“Parent Category” and Subcategory”) were created, and the value was retrieved from column “Category and Subcategory”  were created,
-	To round the value in column “Percentage Funded” with standard rule, the following formula was used: =ROUND(E2/D2*100,0), 
-	Unix epoch time, in the dataset was converted into Excel’s date format (6/22/15) by using the following formula: =(((J2/60)/60)/24)+DATE(1970,1,1), and two extra columns were added (“Date created conversion” and “Date ended conversion”),
-	Column “Average Donation” was created, and the following formula was implemented =IFERROR(B2/E2,0), 
-	=YEAR() function was used to retrieve a year corresponding to the date (6/22/15), and column “Year” was added .

As long as the dataset of Kickstarter campaigns illustrates lots of categories which are not related to plays, analysis had to be condensed by creating pivot tables. And, in accordance with the purpose of the project, correlation between outcomes and two specific factors (Launch Date and Funding Goals) was analyzed.
### Analysis of Outcomes Based on Launch Date
After condensing the dataset, the following Pivot Table was created. 

# PT_1.png
This table shows that during the period from 2009 to 2017, 1369 theater campaigns were launched and 839 of them were successful, which constitutes about 61%. Whereas, 36% and 3% are failed and canceled campaigns, respectively. Among month, May and June has the most successful campaigns launched. It will be better illustrated in the following Pivot Chart.
# Pivot Chart
Looking at the chart it is clear that quantity of both successful and failed campaigns reached their maximum points in May. After that, quantity of successful campaigns started falling gradually. Whereas the quantity of failed campaigns remained stable till August. In December, successful campaigns hit a low, and it was almost on the same level with failed campaigns. Also, it is urgent to state the quantity of failed campaigns always fluctuated between 31 and 52. And, the quantity of canceled campaigns was never over 7. Therefore, it is not significant in the analysis.



### Analysis of Outcomes Based on Goals
Now, it is time for correlation between outcomes and goals. The following Pivot Table illustrates how campaigns with different funding goals succeeded. 

i[Pivot Table - Outcome based on Goal](Resources/Images/PT_2.png)







As it can be seen that the number of successful campaigns is the most in the range between $1,000 to $4,999 (388 campaigns). And, the number of campaigns with 
over $5,000 is 

  the quantity of campaigns with successful campaings of successful funding goals of 534 campaigns are between $1000 and $4999. Also, it should be stated that as the amount funding goals rises the quantity of successful campaigns falls. Number of outcomes




-	=COUNTIFS(Kickstarter!$D:$D,"<1000",Kickstarter!$F:$F,"failed",Kickstarter!$R:$R,"plays") 
-	=SUM(B2:D2) 


-	to the dataset of Kickstarter campaigns was further organized by using the following formulas Two columns “Parent Category” “Category and Subcategory” was divided into 

### Challenges and Difficulties Encountered

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

- What can you conclude about the Outcomes based on Goals?

- What are some limitations of this dataset?

- What are some other possible tables and/or graphs that we could create?
