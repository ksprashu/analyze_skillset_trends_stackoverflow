# Programming Language Preferences

## Background
This data analysis was done as part of a project for a **Data Scientist Nanodegree** that I am pursuing on **Udacity**.

The jupyter notebooks associated with this project and blog post can be [found on GitHub](https://github.com/ksprashu/analyze_skillset_trends_stackoverflow).

Stackoverflow has been doing developer surveys for at least the last 9 years. They have been gracious enough to share the anonymised dataset of these surveys on the public domain for Data Science students like me to analyse. Links to the data sets can be found on the readme in the Github repo.

## Introduction
As a programmer myself and having learnt and coded in over a dozen languages in the past decade, I was interested in some objective data on how the programming languages are changing in their popularity over time. It is just 9 years of data, but I wanted to see if there were any interesting trends that I could pick up, such as new languages that became popular, or evergreen languages that stood the test of time. I also wanted to see if I could bring out any correlation between the languages and the salaries as declared by the respondents. 

What follows are some of the questions that I posed while doing the data analysis and an interpretation of the resultant visualization. To see the data analysis steps that I performed to get at these results, please refer to the jupyter notebooks in the github repo.

## Data Analysis
### Which languages are the most popular?
In order to answer this question, I had to first understand the languages being surveyed. 

![Number of respondents by the year](ds01_yearly_respondents.png)
Up until 2014 there were only about 8000 respondents, whereas in 2015 this jumped to 25000, and to above 60000 in the subsequent years. 

![Number of languages being surveyed every year](ds02_yearly_langs.png)
During the initial few years, until 2014, a relatively smaller number of languages were being surveyed - around 10. In the more recent years a very large number of languages were surveyed - above 40. There were also 'other' languages that the respondents could answer in free text, but since the occurance of that was quite small in comparison to the named languages, I decided to ignore them in the data set.

Based on the the above two data points, I decided to select the data from the years 2015 and above as there were a lot more data points that I could use in order to make a meaningful analysis.

![Top 13 languages](ds03_top13_langs.png)
We can see that Javascript clearly dominates in the amount of usage. This shouldn't come as a surprise as Javascript is popular across the full stack - both in frontend engineering as well as backend engineering and hence the reach is wider. In addition, with the ease of use and increase in adoption of Node.js the usage of Javascript has grown all the more.

The second most popular language is SQL. This one came as a pleasant surprise to me. With so much increase in popularity of NOSQL as well as tools and libraries that abstract you away from SQL, it is still good to see so many respondents still writing SQL in their professional career. 

Java and C/C++ are still popular as every showing that a lot of code in the world is still being written in these 'traditional languages'. .Net/C# is very popular as well showing that Windows technologies are still popular considering the large amount of PC users. Scripting languages are popular too with Python and PHP factoring in the top 6.

I specifically want to call out the 3 languages / frameworks - Typescript, React.JS, and .Net which were only surveyed in the last 3 years of the survey, but are showing how their popularity has been increasing in recent times as their usage is on par with the more stable languages from the top 10. We'll know more about these 3 as we see their year-on-year growth.

### How have the languages grown year-on-year?
![Growth of languages](ds04_lang_growth.png)
5 languages are showing a strong linear growth since 2017 - Javascript, SQL, Java, Python, and Node.js. Java seems to be a little muted in 2019 which has allowed Python to overtake it in terms of popularity displacing it from the 3rd position.

3 upstarts that were introduced in the survey in 2017 - React.js, Typescript, and .Net are showing a very strong linear growth as well. Interestingly, .Net didn't show any change between 2017 and 2018, but suddenly took off in 2019 - did Windows suddenly gain popularity (maybe due to the Surface devices?) or was there some other compelling event?

Most of the other languages have plateaued and are not showing any YoY growth, including the bottom 3 languages - Visual Basic, Objective-C, and Ruby.

### Do certain languages help developer earn more, or vice versa?
We have a broad spectrum of salaries for the respondents who have chosen to answer. We also have salaries as answered by respondents from 2011 up until 2019. Clearly the salaries in 2019 will be much more higher than than salaries in 2011 for the same respondents. We do not have the salaries adjusted for growth, hence we will consider only the salaries from 2017 and later which is a comparable period.

I have further filtered for data showing the highest salary range (salaries above $120K) and the lowest salary range (salaries below $20K) for analysis.

Finally, I processed the data to show the change in usage between when it appears in the highest salary range as compared to the lowest salary range.

![Usage change between max and min salary ranges](ds06_use_change_sal.png)
Taking the top 13 highest positive and negative changes, we can see that there are some interesting patterns. 

Among the languages where the usage has grown, we see Ansible, Chef, and Puppet among others. Dev Ops seems to be one of the high paying job categories with skills growing in demand.

Cloud, and cloud-scale related technologies like SalesForce, Cassandra, and Spark are also seeing more usage in the higher salary ranges.

On the flip side, PHP and related frameworks - like Laravel, Drupal, and Wordpress are the biggest losers showing the largest drop in usage among the highest paid respondents. It does look like maintaining and developing on PHP and products built on PHP are relevant for entry level jobs and there isn't significant salary growth there.

Surprisingly, JQuery, Flutter, and Firebase are among the losers as well. On a whole there aren't enough takers for web technologies as it seems.

Game development too doesn't seem to be on the higher end of the payscale with usage of frameworks like Unreal Engine, Unity 3D, and CryEngine finding reduced usage in the higher salary ranges.

## Conclusion
This is great data that has been collected and provided by StackOverflow. There are various ways that this data can be sliced and diced, however some of they key inferences that I have made are

1. Well known languages such as Java, C++, and Python are still significant in today world and also command high salaries. A significant chuck of development is still being done on these languages, and those new to programming cannot go wrong with them. In fact one of more of these are a must in a  programmer's repertoire. 

2. Usage of Languages and Technologies also rally around industry trends such a Cloud, Dev Ops, and Full-stack development. Technologies related to these are increasingly becoming popular.

3. Frontend development and Game development aren't as money making it seems. On the frontend stack, it is mostly the outdated technologies like PHP that are showing a drop in adoption. On the game development side, the skills are quite niche and newer engines are being used, but it needs to be further investigated why there isn't as much salary growth. 
