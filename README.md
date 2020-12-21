# Kickstarting with Excel
## 1. Overview of Project
### Purpose
The purpose of this project was to uncover trends in campaign fundraising to help Louise maximize her chances of getting her play fully funded. She specifically was interested in learning more about how various campaigns managed relative to both their launch dates and their funding goals. 
## 2. Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
To analyze outcomes based on launch date, I created a pivot table with the months of the year broken down into successful, failed, and canceled campaign outcomes. I then broke this down further the theater category. 
![image](This_PC/Pictures/Launch_date.png)
I then created a line graph that showed the results visually. Looking at the graph it was clear that more successful campaigns were launched during the summer and the least successful campaigns launched during the winter. 
 
### Analysis of Outcomes Based on Goals
To see outcomes based on goals, I created a table that broke down the goal total amounts into $5k increments starting from under $1k and going to greater than $50k. I ran a COUNTIFS function to find the number of successful, failed, and canceled plays by goal amount. 
For example, to find the number of successful plays whose goal ranged between $1000 and $4900 I ran the function below: 
=COUNTIFS(Kickstarter!$D:$D, ">=" & 1000, Kickstarter!$D:$D, "<=" & 4999, Kickstarter!$F:$F, "successful", Kickstarter!$R:$R, "plays")
 
Next, I totaled the projects across the rows and created a percentage by dividing the total number by the outcome category. Finally, I graphed these findings by highlighting the Goal column as well as the percentages columns and clicking ‘insert line graph.’
 
### Challenges and Difficulties Encountered
I had difficulties figuring out how to create the ranges in the COUNTIFS function. I googled how to write the function so that the sheet would pull the numbers I was looking for from the other sheet. 
## 3. Results
- What are two conclusions you can draw about the Outcomes based on Launch Date?

The most successful month to launch your campaign in is May. The least successful month to launch your campaign is December. 
- What can you conclude about the Outcomes based on Goals?

Campaigns under $5000 are the most successful. Campaigns of $45000 and above are the least successful. 
- What are some limitations of this dataset?

The dataset is rather small and therefore not as accurate as it would be if we had more plays to look at. It also is dated with the most recent entries from March of 2017. It is difficult to answer the “why” questions with just this excel sheet. For example, why are campaigns are more successful in May. 
- What are some other possible tables and/or graphs that we could create?

We could see which country preformed better by selecting for US and BG as Louise was also thinking of having her play in the UK. We could see if duration made a difference in how long a campaign should run in order to have the best outcomes. We could create a table showing the average donation relative to each subcategory and sort by descending to see which industry has the most generous donors. Then perhaps make a play about that industry and invite them to the Kickstarter. 
