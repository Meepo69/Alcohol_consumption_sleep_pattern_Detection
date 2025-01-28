# Alcohol Consumption vs Sleep Pattern Detection

## Project Overview
The goal of this project is to explore and analyze the relationship between alcohol consumption patterns and sleep behaviors. The dataset consists of information on alcohol usage and sleep disorders. We aim to understand how alcohol frequency and the average amount of drinks consumed per day correlate with sleep patterns and trouble sleeping.

## Features
- **Data Cleaning**: Handles missing values, selects relevant columns, and renames them for clarity.
- **Feature Engineering**: Creates new features such as average sleep hours across weekdays and weekends, and a binary column for trouble sleeping.
- **Statistical Analysis**: Pearson correlation and T-test to analyze relationships between alcohol consumption and sleep patterns.
- **Visualization**: Various visualizations like distribution plots, scatterplots, boxplots, and correlation heatmaps to illustrate insights from the data.

## Objectives
- Explore the relationship between alcohol consumption and sleep patterns.
- Analyze the impact of alcohol frequency and average drinks per day on sleep quality.
- Visualize key patterns and correlations in the dataset.
- Perform statistical analysis to draw conclusions and validate hypotheses.

## Technologies Used

### Frameworks and Libraries
- **Python**: Primary programming language for data manipulation and analysis.
- **pandas**: For handling and cleaning data.
- **pyreadstat**: For reading SAS Transport files (.XPT format) into pandas DataFrames.
- **matplotlib**: For data visualization (e.g., scatterplots, boxplots).
- **seaborn**: For enhanced statistical graphics (e.g., heatmaps).
- **scipy**: For statistical analysis (e.g., Pearson correlation, T-tests).
- **Jupyter Notebooks**: For development and exploratory data analysis.

### Model Architecture & Deployment
- **Data Cleaning**: Removed missing values, selected relevant columns, and renamed for clarity.
- **Feature Engineering**:
  - Created a new feature for the average sleep hours across weekdays and weekends.
  - Transformed the "Trouble Sleeping" column into a binary format (0 = No, 1 = Yes).
- **Statistical Analysis**:
  - Performed Pearson correlation to examine the relationship between alcohol consumption and sleep hours.
  - Conducted a T-test to compare sleep hours between individuals with trouble sleeping and those without.
- **Visualization**: Various visualizations created to examine the relationship between alcohol consumption and sleep:
  - Distribution of alcohol consumption frequency.
  - Scatterplot of average drinks per day vs. average sleep hours.
  - Boxplot of sleep hours categorized by trouble sleeping status.
  - Correlation heatmap for relevant features.

## Dataset and Preprocessing
- **Dataset**: The data is sourced from two datasets:
  - **ALQ_J (Alcohol Use)**: Contains information on alcohol consumption frequency and the average number of drinks consumed per day.
  - **SLQ_J (Sleep Disorders)**: Contains details about sleep hours on weekdays and weekends, along with indicators of trouble sleeping.
  
- **Preprocessing**:
  - Missing values were removed from both datasets.
  - Columns were renamed for clarity and relevance.
  - The datasets were merged on a common identifier (`SEQN`).
  - A new feature for the average sleep hours across weekdays and weekends was created.
  - The "Trouble Sleeping" column was converted to a binary format.
  
## Training Details
- **Data Exploration**: Basic statistics and initial visualizations were created to understand distributions and relationships between alcohol consumption and sleep behavior.
- **Model Optimization**: This project does not involve machine learning models but focuses on exploratory data analysis using statistical techniques.
- **Interpretability**: Visualizations such as heatmaps and scatterplots were used to provide clear insights into relationships between variables.

## Deployment Instructions

1. **Environment Setup**:
   - Install the necessary libraries using the following:
     ```bash
     pip install pandas matplotlib seaborn pyreadstat scipy jupyter
     ```
   
2. **Running the Code**:
   - Clone the repository and open the notebook in Jupyter to run the code.
   - The dataset `ALQ_J.XPT` and `SLQ_J.XPT` must be available in the working directory.
   
3. **Visualizations**:
   - Run the code to generate the visualizations for alcohol consumption vs. sleep patterns and the statistical analysis results.

## Challenges and Solutions

### Challenges
1. **Data Variability**: Variations in alcohol consumption and sleep behavior could complicate analysis.
2. **Data Cleaning**: Ensuring consistency in column names and handling missing values required detailed cleaning.
3. **Interpretability**: Visualizing complex relationships between multiple variables can sometimes obscure key insights.

### Solutions
1. **Data Imputation**: Missing values were handled by removing the rows to ensure accurate analysis.
2. **Statistical Techniques**: Pearson correlation and T-tests were applied to draw meaningful insights from the data.
3. **Visualization**: Clear and easy-to-interpret visualizations were created to represent complex data relationships.

## Future Work
- **Data Expansion**: Include additional features such as weather conditions, mental health data, and demographics for more in-depth analysis.
- **Predictive Models**: Implement machine learning models to predict sleep issues based on alcohol consumption and other features.
- **Real-Time Data Integration**: Incorporate real-time data from external sources to analyze live alcohol consumption patterns and sleep behavior.

## How to Use
1. Clone the repository.
2. Install the necessary dependencies.
3. Load the dataset (`ALQ_J.XPT` and `SLQ_J.XPT`) into the notebook.
4. Run the provided Jupyter notebook to explore the data, perform statistical analysis, and visualize the results.
5. Interpret the insights from the visualizations to understand the relationship between alcohol consumption and sleep patterns.

## Contact Information
**Author**: Atharva Talegaonkar  
**Email**: atale014@ucr.edu
