# Kickstarting with Excel

## Overview of Project
Analysis of kickstarter data to support a new kickstarter project.

### Purpose
To analyze kickstarter fundraising data by outcomes based on launch date and goals to inform decision maker in support of her own kickstarter project.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
To analyze the outcomes by launch date, I created a pivot table in Excel and added the outcomes data to the Columns and Values fields; the Date Created Conversion data to the Rows field, and Parent Category and Years to the Filter field. 

I then visualized it by creating a Line with Markers chart with months on the x axis and count of outcomes on the y axis.

![Launch Date Line Chart](https://user-images.githubusercontent.com/106203262/173389415-8bc24060-0984-41bd-a638-c4d6e715f200.png)

### Analysis of Outcomes Based on Goals
To analyze the Outcomes based on goals, I first had to obtain the number of successful, failed, and canceled kickstarters based on a range of the goal amount. To do so, I used a =countifs function to search the corresponding worksheet and column and count the number of rows that contained a value within the defined parameter. Once I obtained the counts, I then calculated the percentage that each range either succeeded, failed, or canceled. To do so, I divided the number of the individual field by the total count for that range.

I then created a Line with Marker chart to visualize this information by placing the goal ranges in the x axis and the percentage on the y axis.

![Parent Category Outcomes Bar Chart](https://user-images.githubusercontent.com/106203262/173389524-d813bbb5-3112-4f3b-906b-c3dbd0cbb540.png)

### Challenges and Difficulties Encountered
I did not face any challenges in creating the pivot table or chart, but depending on the data I had, a line chart might not have been the best and I could envision scenarios where I would have had to try different chart types to see which one best visualized the information I wanted to present.

The only challenge I faced in conducting the outcomes based on goals analysis was ensuring that the Number Canceled counts were truly zero. At first this seemed odd, so I went back into the original kickstarter data to verify that it was correct. I filtered the subcategory column to plays and the outcomes column to canceled to do so.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
Based off this analyzed data set, it can be concluded that the best time to start a theater kickstarter for the highest rate of success is in May. It can also be concluded that theater kickstarters are more often successful than they fail.

- What can you conclude about the Outcomes based on Goals?
Based off this analyzed data set, it can be concluded that for the most part, with an exeption, the lower the goals amount, the higher the success rate. However, this is not absolute as there are two data points in the $35,000 to $45,000 point that do not follow this trend. More analysis would be required to explain this, but initially it seems the count for those levels are extremely low and possibly outliers. It can also be concluded that at the $15,000 to $19,999 range both the success and fail categories are 50%, suggesting this may be the maximum amount a decision maker may want to decide on a goal to ensure the risk of failure is not higher than success.

- What are some limitations of this dataset?
We did not identify outliers that may be skewing the analysis. This may be the cause of the $35k to $45k data points having a higher success percentage that probably found in a larger sample size. 

- What are some other possible tables and/or graphs that we could create?
I'd be interested in combining both the launch by date data with the outcomes based on goals to see if I could get better fidelity into which month and goal amount would give me the best success odds.
