# Analysis of trends in Skillset data from Stackoverflow

## Data Acquisition
The datafiles for this analysis have been obtained from StackOverflow at [this link](https://insights.stackoverflow.com/survey). The jupyter notebooks in this repo will help you download the data files and extract the relevant data from them.

## Objective
In this analysis, we would like to take a look at the data sets of the stackoverflow surveys held year on year from 2011 to 2019 and see how the trends are changing year on year. 

Specifically I would like to look at trends in programming languages and technology and compare it to salary of the individuals working on those technologies, where possible.

## Installation
The jupyter notebook will run on a default installation of Anaconda. It is not necessary to install any additional modules for the purpose of running this code. 

The pre-requisite files will be downloaded by the script when run the first time.

## File Description
There are 3 files as part of this repository.

### acquire_files.pynb
This file is meant to be run first and as a one time activity. The file will download all the pre-requisite resources and datasets from stackoverflow and place them in the filesystem so that the other notebooks can use this data to do the analysis.

### wrangle_data.pynb
This file will load the csv files that were downloaded and extract the required features from those datasets. Then it will combine all the data and export it for further analysis.

### analyze_tech_trends.pynb
This file will load the consolidated dataset of the programming language usage and do all the relevant data analysis to look for answers to the questions posed.

## Results
The findings during this analysis and the results thereof have been all documented in [this blog post on medium](https://medium.com/@ksprashu/programming-language-preferences-7e9bfed0f5d1)

## Adaptations of Work
<none>

## License and Acknowledgements
- The data was sourced from [Stackoverflow](https://insights.stackoverflow.com/survey). Due credit to stackoverflow for running such a comprehensive study year and year and further for making this data available for public access.
- All work and analysis on top of this data was solely created by @ksprashu; however feel free to use this repo, the accompanying blog, and the jupyter notebooks as you would please as long as due credit is extended.
- If you do do more data wrangling and are able to clean up the data further for better actionable analysis, feel free to send me pull requests to merge the changes. You can even send me the repo urls so that I can add it to the adaptations of this work for those ineterested in exploring further.

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

### Websites as reference
- https://techoverflow.net/2018/01/16/downloading-reading-a-zip-file-in-memory-using-python/
- https://docs.python.org/3/library/zipfile.html
- https://matplotlib.org/contents.html
- https://seaborn.pydata.org/api.html
and of course
- https://stackoverflow.com/
- https://insights.stackoverflow.com/survey
