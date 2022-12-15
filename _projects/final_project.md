---
name: Final Project Part 3
author: Trevin Kurniawan
tools: [Python, HTML, vega-lite]
description: This project showcases crashes in the city of Chicago

remote_projects:
   -online_cv_public

custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---
# Crash Reports in Chicago

Author: Trevin Kurniawan

For this final project, I want to use a dataset from the City of Chicago Data Portal. This dataset contains informations abour car crashes that occured in the streets of Chicago named :"Traffic Crashes - Crashes". The data is from the "electronic crash reporting system (E-Crash) at CPD". This dataset is owned by the Chicago Police Department.

The license can be found in [Chicago Car Crashes](https://www.chicago.gov/city/en/narr/foia/data_disclaimer.html), it contains the Terms and Conditions of how the data needs to be used. The department still have rights for this data since it is stated that "The City may require a user of this data to terminate any and all display, distribution or other use of any or all of the data provided at this website for any reason including, without limitation, violation of these Terms of Use or other terms as defined by City agencies or departments contributing data to this website.", also the website wants that every user to provide a disclaimer “This site provides applications using data that has been modified for use from its original source, www.cityofchicago.org, the official website of the City of Chicago. The City of Chicago makes no claims as to the content, accuracy, timeliness, or completeness of any of the data provided at this site. The data provided at this site is subject to change at any time. It is understood that the data provided at this site is being used at one’s own risk.”

This project is based on a dataset from the police department of Chicago. It shows many records and details of car crashes that happened in the city of Chicago and this is the raw URL of the dataset. For this project, I have trimmed the sample size since the original dataset contains thousands of datas. The reason I trimmed the data is because it will take too long to process all the data and Starboard is unable to process that much amount of data. Therefore I will be using the link below for my research. I have made analysis using the original dataset and the trimmed dataset.
[Car Crashes in Chicago](https://raw.githubusercontent.com/hollow27mc/IS445-Final-Project/main/Traffic_Crashes_-_Crashes.csv) 

# Contextual and Interactive Visualizations

We will be using vega-lite to plot the count of car crashes in different weather conditions. We are also going to be using a bar graph; this visualization will showcase the trend of car crashes according to the weather conditions. I chose Red as the hover color because red color is one of the sharpest color to attract attention and drivers need to pay full attention when they are driving in order to avoid accidents.

---
<vegachart schema-url="{{ site.baseurl }}/assets/json/weatherCrashes.json" style="width: 100%"></vegachart>
---
The visualization below utilizes vega-lite again to plot the count of car crashes in different speed limits. We will again be using a bar graph; this visualization showcase the trend of car crashes in 30mph speed limit roads. I tend to choose green as the hover color because it contrast the steelblue color of the bar graph and green usually presents the word "go".
---
<vegachart schema-url="{{ site.baseurl }}/assets/json/speedlimit.json" style="width: 100%"></vegachart>
---
The next visualization also uses vega-lite. It showcases the amount of car that crashes according to the month and street direction of the accident. User can click and choose the direction (North, East, West and South) and also the month (1 - 12).
The visualization will show the amount of car crashes during the month by using colors, Dark Blue will be the highest amount of crashes and Light Green means that it has the least amount of crashes.
---
<vegachart schema-url="{{ site.baseurl }}/assets/json/Direction_crashes.json" style="width: 100%"></vegachart>
---

# Conclusion

I hope that these visualization can help people to be more cautious with their surroundings especially when they are driving. In the first visualization we can see that even most car accidents happen during the clear sky. The second visualization shows that even only going 25mph, accidents can happen. Third visualization shows that most car accidents in happened during the summer in Chicago. This shows that accidents can happen anytime and anywhere, I hope that people will be more aware with their surroundings and drive safe.

# Citations
https://www.chicago.gov/city/en/narr/foia/data_disclaimer.html
www.cityofchicago.org
https://www.chicago.gov/city/en.html
