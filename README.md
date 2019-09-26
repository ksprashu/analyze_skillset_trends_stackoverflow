# Analysis of trends in Skillset data from Stackoverflow

## Data Acquisition

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
This file will load the consolidated dataset of the programming language usage and look for year on year trends and how they compare to the compensation.

## Results

## License and Acknowledgements
- The data was sourced from [Stackoverflow](https://insights.stackoverflow.com/survey). Due credit to stackoverflow for running such a comprehensive study year and year and further for making this data available for public access.
- All work and analysis on top of this data was solely creaated by @ksprashu; however feel free to use this repo, the accompanying blog, and the jupyter notebooks as you would please as long as due credit is extended.

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

### Websites as reference
- https://techoverflow.net/2018/01/16/downloading-reading-a-zip-file-in-memory-using-python/
- https://docs.python.org/3/library/zipfile.html
