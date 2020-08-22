# PythonForAnalytics-Grp4
Python for Analytics Group 4 Project Code Repository

## Final Project Location and Name



<h1>Table of Contents<span class="tocSkip"></span></h1>
<div class="toc"><ul class="toc-item"><li><span><a href="#PythonForAnalytics-Grp4" data-toc-modified-id="PythonForAnalytics-Grp4-1">PythonForAnalytics-Grp4</a></span><ul class="toc-item"><li><span><a href="#Final-Project-Location-and-Name" data-toc-modified-id="Final-Project-Location-and-Name-1.1">Final Project Location and Name</a></span></li><li><span><a href="#Package-Setup" data-toc-modified-id="Package-Setup-1.2">Package Setup</a></span></li><li><span><a href="#Project-Members" data-toc-modified-id="Project-Members-1.3">Project Members</a></span></li></ul></li><li><span><a href="#Detailed-Requirements" data-toc-modified-id="Detailed-Requirements-2">Detailed Requirements</a></span><ul class="toc-item"><li><span><a href="#Outline-(from-Canvas)" data-toc-modified-id="Outline-(from-Canvas)-2.1">Outline (from Canvas)</a></span></li><li><span><a href="#Requirements" data-toc-modified-id="Requirements-2.2">Requirements</a></span></li><li><span><a href="#Ethics" data-toc-modified-id="Ethics-2.3">Ethics</a></span></li><li><span><a href="#Deliverable" data-toc-modified-id="Deliverable-2.4">Deliverable</a></span></li><li><span><a href="#General-notes" data-toc-modified-id="General-notes-2.5">General notes</a></span></li><li><span><a href="#Here-are-some-interesting-notebooks-I-found-online" data-toc-modified-id="Here-are-some-interesting-notebooks-I-found-online-2.6">Here are some interesting notebooks I found online</a></span></li></ul></li><li><span><a href="#Process-Outline" data-toc-modified-id="Process-Outline-3">Process Outline</a></span></li><li><span><a href="#Individual-Analysis-Notebooks" data-toc-modified-id="Individual-Analysis-Notebooks-4">Individual Analysis Notebooks</a></span><ul class="toc-item"><li><span><a href="#Shyan-DasMadan" data-toc-modified-id="Shyan-DasMadan-4.1">Shyan DasMadan</a></span></li><li><span><a href="#Sam-Gunther" data-toc-modified-id="Sam-Gunther-4.2">Sam Gunther</a></span></li><li><span><a href="#Prafulla-Ranjan-Dash" data-toc-modified-id="Prafulla-Ranjan-Dash-4.3">Prafulla Ranjan Dash</a></span></li><li><span><a href="#Brandon-Carp" data-toc-modified-id="Brandon-Carp-4.4">Brandon Carp</a></span></li></ul></li><li><span><a href="#Supporting-Technology" data-toc-modified-id="Supporting-Technology-5">Supporting Technology</a></span><ul class="toc-item"><li><span><a href="#Packages" data-toc-modified-id="Packages-5.1">Packages</a></span></li><li><span><a href="#Jupyter-Notebook-Extensions" data-toc-modified-id="Jupyter-Notebook-Extensions-5.2">Jupyter Notebook Extensions</a></span></li></ul></li></ul></div>

## Project Members

Brandon Carp
Shyan DasMadan
Sam Gunther
Prafulla Ranjan Dash

# Detailed Requirements

## Outline (from Canvas)

You and your teammates form a  journalism department. Your task is to provide interesting insights or analysis based on the file listed below. 

Instead of worrying about "staying within the lines," be creative in how look for insights and in how you present them. In that sense, this is a very easy assignment. As long as you fulfill the requirements, you will get full marks for this assignment. 

However, your final notebook, containing your names, will be shared with all of your classmates (who will be asked to not share it publicly).

I expect your final notebook to at least contain basic exploration of data. At least basic data cleaning. I expect you to show some interesting insights you were able to glean from the data set, supplemented with visual charts.

## Requirements

- Download file from https://www.foreignlaborcert.doleta.gov/performancedata.cfm#dis the latest version PERM "FY2020 Q3.xlsx"
    - Data dictionary available under "PERM Record Layout.pdf" link
- Form groups of three and explore the data
    - Do quick exploration of data
        - Create histograms of variables
        - Pay attention to which ones you like
        - Investigate data exploration tools, some ideas: 
            - pandas profiling https://github.com/pandas-profiling/pandas-profiling
            - dabl https://amueller.github.io/dabl/dev/index.html (from one of the core contributors of Scikit-Learn)
            - t hink about joining other datasets to augment this file
    - Come up with ideas about what you want to explore. Potential ideas:
        - Which cases are more likely to succeed given a profession, city, lawyer, filing date?
        - Use tf/idf or word vectors or whatever to summarize professions (NLP)
        - What are the top newspapers for each city vs profession (blue collar vs white collar)
        - Don't try to investigate everything! Pick a direction, let other teams follow their own paths
    - Clean/normalize the data. Potential ideas:
        - missing values?
        - pay in terms of hourly vs annual?
        - why are some descriptions all caps?
    - Clearly communicate results. 
        - Use lessons from "Leadership" class (if you've taken it)
        - But use jupyter, not power point (unless you want to use the RISE plugin for Jupyter or something similar)
        - Create nice visualizations (optional)
     - You must use GitHub to manage this project and coordinate among your teammates 
        - This should be very helpful: https://github.com/jupyterlab/jupyterlab-git
        - This is an alternative, probably not as user friendly https://github.com/jupyter/nbdime
    - Since this is a team project, you must come up with a good methodology for managing changes, here are some suggestions:
        - http://drivendata.github.io/cookiecutter-data-science/
        - https://github.com/quantumblacklabs/kedro
        - Just give these links a quick read. You don't have to install any packages. Just pay attention to their recommendations.
            - Pay attention to their directory structure and how they organize their notebooks, data assets, etc.
            - Pay attention to how they name their files
            - Pay attention to what other lessons you can learn from them, but trying to follow every suggestion will likely be a waste of time for such a short project

## Ethics

- This data contains LOTS of private information. Use it with care.
    - Would you still be ok if your analysis became public, perhaps viral?
- Expect your anaysis to be challenged. Challenge the analysis of other teams

## Deliverable

- I expect one main python notebook containing your analysis
- You can upload a zipped folder which contains supporting notebooks which contain
    - Your basic exploration
    - Experiments you may have done
    - A README file telling me where to find the main notebook
    - Everything, except the main notebook is optional

## General notes

- You may use any package and learn from anyone (classmates, resources on the internet), but may not directly copy
    - Feel free to reach out to your colleagues to see what they are doing. Set up zoom calls for walkthroughs of each other's work
    - Investigate visualization packages, some ideas to get you started: matplotlib, seaborn, altair, bokeh, holoviews, bqplot
- You do not have to build prediction or clustering models, but you may build several if you like
- You can "hire" me to provide extra lectures on version control, visualization or any other topic. The cost is that you must convince at least 8 people to attend this extra lecture. 

## Here are some interesting notebooks I found online

- Notebook which is nicely done, although it is in French:
    - https://github.com/jhroy/theses/blob/master/theses.ipynb
- World differences in infectious tuberculosis prevalence:
    - https://github.com/jadianes/data-journalism/tree/master/articles/tuberculosis-world-situation
- Exploring Datasets with Python:
    - https://github.com/MartinSeeler/python-data-exploration/blob/master/Exploring%20Datasets.ipynb

# Process Outline

1. Reviewed the dataset and data dictionary.
1. Agreed to focus the analysis on the differences between applications that are approved versus applications that are denied, in an effort to draw insights as to why certain applications might be denied.
1. Reviewed the dictionary again, using the spreadsheet `PERM_FY2020_Q3_feature_list.xlsx` to divide up each feature for our individual analyses.
1. Agreed to base analysis off `CASE_STATUS_BINARY` to ensure each group member was dividing "Denied" versus "Certified" consistently.
1. Conducted individual analyses and met again to discuss insights and share ideas for enhancements and further exploration. Each individual analysis is located in root GitHub location for the project, and their names are identified under each group member's name in `Assigned Features.ipynb`.
1. Used completed individual analyses to draft consolidated report for review and submission. Final report name is ``.

# Individual Analysis Notebooks

## Shyan DasMadan

`Labor Analysis - DasMadan.ipynb`

## Sam Gunther

`Labor Analysis - Sam Gunther.ipynb`

## Prafulla Ranjan Dash

`Training and Skills Analysis - Prafulla.ipynb`

## Brandon Carp

`PERM Analysis - Brandon Carp.ipynb`

# Supporting Technology

## Packages

- numpy and pandas - used for basic data cleaning and exploration
- matplotlib and seaborn - used for data exploration
- datetime - used to parse dates to allow for time series analysis

## Jupyter Notebook Extensions

- Table of Contents (2) - Allows notebook to use headers to assemble table of contents that can be displayed both in-notebook and as a separate window/spine
