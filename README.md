# matplotlib-challenge

A company named **Pymaceuticals** who specializes in anti-cancer pharmaceuticals. In its most recent efforts, it began screening for potential treatments for squamous cell carcinoma (SCC), a commonly occurring form of skin cancer.

### Source Files
* There are two source files available for the analysis. One file contains all the information about mice that are used in the stud, the second file contains the study information.

### Data Preparation
* The two raw source files have been combined into one file
* I have assumed that each entry should have an unique pair of "Mouse ID" and "TimePoint". Therefore all entries in the dataset with the same pair "Mouse ID" and "TimePoint" have been identified as duplicate values. 
* I have cleaned the data by using two methods:
    1) Finding duplicate values then keeping only one of them. However, I noticed that Tumor Volume wasn't the same for some entries with the same pair of "Mouse ID" and "TimePoint". Therefore, I decided to use the second method
    2) Instead of dropping duplicate values all together, I decided to combine them by averaging Tumor Volume for the duplicate values. Again, duplicate values have been defined as entries with the same pair of "Mouse ID" and "TimePoint". Once the operation was performed I named the new Data Set as clean_df and used it for further analysis

Please refer to the [Analysis Jupyter Notebook](./pymaceuticals.ipynb) for conclusions and the details of the analysis