# kickstarter-analysis

Kickstarting with Excel

Overview of Project

Purpose
This project was completed for our aspiring playwright friend, Louise, who is attempting to fund her self-produced play, “Fever”, through a successful Kickstarter campaign. Our analysis utilized a dataset consisting of thousands of Kickstarters from a wide range of categories,  including pertinent data points such as Goal Amount, Funding Amount, Outcome, Date Launched, Date Ended, and various descriptive data about the title, location, and category of the campaign.

Analysis and Challenges

Analysis of Outcomes Based on Launch Date

Louise was especially curious about the effect that Launch date could have on her campaign. We provided her with actionable intel by performing an analysis of all campaigns in the data set to determine the outcome of each Kickstarter based on its launch month. These results were gathered in a pivot table in Excel, and can be further filtered by year and parent category, allowing us to parse the relatable data and uncover trends for similar projects. The following chart provides a breakdown of all projects in the “Theater” parent category, showing the results of the campaigns by Launch Date.
![Theater_Outcomes_vs_Launch_Date](https://user-images.githubusercontent.com/100643755/160319023-ae7e6d6a-1854-4343-99ad-c2c33623b517.png)


Analysis of Outcomes Based on Goals

Another area of interest for Louise was the relationship between funding goal and project outcome. We were able to break down the data for all project under the “Play” subcategory into 12 distinct goal levels, ranging from sub-$1,000 to $50,000 or more. For each of these levels, we calculated the percentage of successful, failed, and canceled projects, and used our results to create the following chart. This chart allows us to quickly identify useful trends and pass on recommendations for project goal to Louise.
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/100643755/160319079-2ed80daa-edc6-44e7-8799-99e3f0f8e21c.png)


Challenges and Difficulties Encountered

While the analysis that Louise requested was mostly straightforward, there were 2 areas that required extra attention to make sure our findings were accurate. First, we needed to manipulate the data to extract useful information in regards to parent- and sub-categories, as well as date and year information from the included epoch timestamps included with the original dataset. Second, the breakdown of project goal levels required the use of the Countifs formula in excel, and required up to four criteria to properly filter the entire dataset and return only our desired results.

Results

From our analysis, we are able to draw two conclusions for Louise in regards to outcomes based on launch date and one conclusion about the outcomes based on goal amounts. These conclusions are as follows:
	- The best time to launch a Kickstart campaign is in May, as it has the highest number of successes (111) while keeping failures (52) at an amount that 	is not significantly higher than that of June (49),  July (50), August (47), or October (50).
	-The worst time to launch a Kickstarter campaign is December, as the number of successful and failed campaign are nearly identical, with only 37 	successful campaigns to 35 failed,  by far the worst ratio of any month.
	- The success rate of a Kickstarter appears to be inversely related to its goal amount. The lowest level of funding in our breakdown (less that $1,000) 	has the highest rate of success(76%). Success rate drops at each successive level up to the $25,000 to $29,999 level. Above this level, success rates do not 	strictly follow the inverse relationship.  However, it is important to note that the sample size at these levels is rather small, making any significant 	conclusions difficult to draw.

Limitations

While the data set we utilized is robust, there are certain limitations that should be kept in mind. The most glaring of these issues is that the data set does not normalize for the native currency of each project. This can potentially undermine the results of our analysis, as exchange rates between currencies constantly fluctuate, and therefor the relative goals of each project are not known. To mitigate this issue, the data set would have to be converted to a single currency, utilizing the launch and end dates of each project to look up and apply the appropriate conversion rate for each project. Another limitation is that the information does not include any insight into the popularity or renown of the creator of each project. It would be easy to assume that creators with a larger social circle (or the ability to advertise their project), would have better success rates than those who are relatively unknown. However, we cannot use such speculation when presenting our analysis to Louise.

Further Recommended Analysis

While we believe that the information we have provided to Louise will greatly help her attempt to run a successful campaign, we also believe she should undertake extra analysis to glean further insights for her current project, as well as any future projects she may wish to run. First, we recommend a pivot table be created that shows the relationship between  backer count, and whether the project was a staff pick or spotlight project. Second, we recommend a chart showing outcomes based on location. Finally, we recommend a table pivot table that shows backer count, outcome, and length of the campaign.
