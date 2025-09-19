# MentorAI_Olymbic_Project

Project Overview
This project analyzes historical Olympic Games data from 1896 to 2016, exploring athlete demographics, performance metrics, and medal distributions. The analysis provides insights into participation trends, athlete physical characteristics, and competitive outcomes across different sports, countries, and time periods.

 Dataset
The dataset used is athlete_events.csv, containing information about Olympic athletes and their performances from 1896 to 2016. The dataset includes:

Athlete Information: ID, Name, Sex, Age, Height, Weight

Team Details: Team name, National Olympic Committee (NOC) code

Event Information: Games, Year, Season, City, Sport, Event

Performance Data: Medal won (Gold, Silver, Bronze, or NaN for no medal)

Technical Implementation
Libraries Used
pandas: Data manipulation and analysis

numpy: Numerical computations

matplotlib: Data visualization

seaborn: Advanced statistical visualization

warnings: Handling warning messages

Key Features
Data Assessment & Understanding

Initial scanning of data structure, shape, and data types.

Crucial Step: Identification and Quantification of Missing Data. A primary goal of this EDA is to understand the scope and pattern of missingness before making any decisions on how to handle it.

Conversion of ID and Year columns to object type for correct categorical handling.

Identification of potential outliers in Age, Height, and Weight columns.

Exploratory Data Analysis (EDA)

Statistical summaries of numerical features (on available data).

Distribution analysis of categorical variables.

Uncovering initial patterns and relationships within the data.

Visualization

Custom color palette implementation.

Medal distribution analysis (bar charts and pie charts).

Demographic analysis of athletes.

Philosophy on Missing Data in this EDA
Why is the data still missing?

This project is an Exploratory Data Analysis (EDA), not a modeling task. The goal of EDA is to understand the data, its structure, and its quirks—not to build a final, production-ready dataset.

Handling missing data (a process called imputation) is a serious step that can introduce bias and alter the fundamental properties of the dataset.

Key Insights
Medal Distribution: Of the athletes who won a medal, there is an approximately equal distribution among Gold (33.6%), Silver (33.0%), and Bronze (33.4%). Crucially, only 14.7% of all athletes in the dataset won a medal, meaning the Medal column has 85.3% missing values (representing "Did Not Medal").

Data Completeness: The dataset contains significant missing data that must be accounted for in any analysis:

Height: 22.2% missing (210,945 / 271,116 entries)

Weight: 23.2% missing (208,241 / 271,116 entries)

Age: 3.5% missing (261,642 / 271,116 entries)

Athlete Demographics (on available data): The average athlete is 25.6 years old, with average height and weight of 175.3cm and 70.7kg respectively. Potential outliers were noted, including an athlete aged 97.
