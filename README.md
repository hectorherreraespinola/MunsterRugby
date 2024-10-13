# MunsterRugby

## Project Overview
This project involved reading rugby match data from XML files using Python, concatenating the data, creating CSV files, importing the data into Power BI, establishing relationships between the data tables, and creating visualizations to analyze the performance of Munster Rugby.

## Steps

### 1. Obtaining and Concatenating XML Data
The initial data was provided in multiple XML files. These files contained detailed information about rugby matches, teams, and fixtures. The first step was to read and concatenate these XML files into a single dataset. This involved parsing the XML structure, extracting relevant data, and combining it into a unified format suitable for analysis.

### 2. Creating CSV Files
After processing and concatenating the XML data, the next step was to save the cleaned and combined data into CSV files. These CSV files were created to serve as the input for Power BI, making it easier to import and manipulate the data within the tool.

### 3. Importing Data into Power BI
The CSV files (`team_data.csv`, `match_data.csv`, and `fixture_data.csv`) were imported into Power BI. This was done by opening Power BI Desktop, clicking on `Get Data`, selecting `Text/CSV`, and importing each of the CSV files.

### 4. Establishing Relationships
Once the data was imported into Power BI, relationships between the tables were established. This was done in the `Model` view in Power BI. The relationships were created based on common columns:
   - `match_data[team_id]` was related to `fix_data[FxHTID]`
   - `match_data[PLID]` was related to `team_data[PLID]`

   ![Model](https://github.com/hectorherreraespinola/MunsterRugby/blob/main/Images/model.png)

### 5. Creating Measures
In Power BI, measures were created to calculate the total carries by Munster Rugby as a home team and as an away team. These measures helped in analyzing the performance of the team in different scenarios.

### 6. Creating Visualizations
Finally, visualizations were created in Power BI to display the calculated measures. Two card visuals were added:
   - The first card displayed the total carries by Munster Rugby as a home team.
   - The second card displayed the total carries by Munster Rugby as an away team.

   ![Dashboard](https://github.com/hectorherreraespinola/MunsterRugby/blob/main/Images/dashboard.png)


## Conclusion
By following these steps, we successfully read rugby match data from XML files, concatenated the data, created CSV files, imported the data into Power BI, established relationships between the data tables, and created visualizations to analyze the performance of Munster Rugby.
 
