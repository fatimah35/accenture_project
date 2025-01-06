# Data Portfolio (Excel - SQL)

![Image](https://github.com/fatimah35/accenture_project/blob/main/assets/images/excel.png)


# Table of Contents
## Objective
## Data Source
## Analysis Tools
## Data Development
#### -Pseudocode
#### -Data Exploration
#### -Data Cleaning
#### -Data Transformation
## DataQuality Checks
## Data Visualisation
## Data Anlaysis
## Recommendations
## Conclusions

# Objective
Accenture have embarked on a 3 month pilot with Social Buzz to focus on 3 main tasks, aligned with some of the biggest challenges thet are currently facing. Social Buzz has reached huge scale in recent years to become recognized as a global unicorn company. Firstly, the team will be doing an audit of your big data practice and sharing best practices and industry expertise. Secondly we will be guiding you through a successful IPO, of which we have deep expertise and knowledge of within our team. And finally, i have conducted an analysis of your data to find insights regarding social buzz's top 5 most popular categories of content.
## Data Source
Data of contents uploaded on social buzz was provided. For this analysis;
-Content ID is needed
-Content Category
-Reaction Type
-Reaction Score
-Content Categogry
-Content Type.
The datasets are attached to the doc file.
# Analysis Tools
| Tool | Purpose 
|------|-------------------------------------------|
|Excel | Exploring the data and visualisation      |                        
| SQL  | Cleaning, testing, and analyzing the data |

# Data Development
## Pseudocode - General approach in creating analysis solution
## -Get the data
## -Explore the data in Excel
## -Load the data into SQL Server
## -Clean the data with SQL
## -Test the data with SQL
## -Visualize the data in Excel
## -Generate the findings based on the insights
## -Write the documentation + commentary
## -Publish the data to GitHub Pages
# Data Exploration Notes - This was the stage i scanned of what's in the data, errors, inconcsistencies, bugs and corrupted characters
- I was provided with three datasets, the reaction dataset,content dataset and reaction types dataset
- There are at least 4 columns in each dataset that contain the data we need for this analysis, which signals we have everything we need from the file without needing to contact the client for any more data.
- We have more data than we need, so some of these columns would need to be removed
# Data Cleaning - The aim is to refine our dataset to ensure it is structured and ready for analysis.
## The cleaned data should meet the following criteria:
## - Contain neccasry columns for analysis
## - Each content id must be unique in the content table(no duplicates)
## - Reaction type must be character,reaction score must be int,content category must be character
## - Column count,unique reactions (16),total reactions recorded after removing blanks (24754)
![Image](https://github.com/fatimah35/accenture_project/blob/main/assets/images/data quality.png)
## Below is a table outlining the featuress of our cleaned dataset:
| Dataet           | Numbers of Columns | DataType                           | Nullable|
|------------------|--------------------|------------------------------------|---------|
| ReactionTypes    | 3                  | Varchar,Varchar, Integer           | No      |
| Reactions        | 4                  | Integer, Varchar, Varchar, Date    | No      |
| Content          | 4                  | Integer, Varchar, Varchar, Varchar | No      |
