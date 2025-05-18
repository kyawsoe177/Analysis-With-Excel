<!---

--->

# Data Cleaning
This dataset contains basic employee information within an organization. It includes the following fields, 'Employee ID', 'Name', 'Date Hired', 'Department', 'Status'. 
The primary focus will be on cleaning this dataset.

## Creating a duplicate
To be safe, we will start by duplicating the dataset in case of any issues.

<img src="https://github.com/user-attachments/assets/d5227737-b976-42db-b2d0-f5717964ff6b" alt="Duplicate worksheet" width="200" height="100">


There are noticeable inconsistencies in the data, including variations in letter casing and the presence of null values.

<img src="https://github.com/user-attachments/assets/7927e839-88dd-41de-b306-4daf1065b969" alt="Messy data" width="400" height="200">


## Cleaning department column
There are missing entries in the 'Department' column. We will apply conditional formatting to highlight these and any other null values.

<img src="https://github.com/user-attachments/assets/eda08ac2-8e78-4ab1-a608-6ef69e6baeae" alt="Conditional formatting" width="100" height="100">

After that, those values will be replaced with 'Unassigned' using the following IF command.
````
=IF(OR(D2="", D2="none"), "Unassigned", D2)
````

## Cleaning duplicates
Identifying duplicate values is also an important step in data cleaning. We will look for duplicates in 'Employee ID' and 'Name' columns with conditional formatting again.

<img src="https://github.com/user-attachments/assets/9aefca06-6fef-46d5-98c3-11e989acd3cc" alt="Conditional formatting" width="200" height="100"><br/>

The duplicate values are highlighted in green.

<img src="https://github.com/user-attachments/assets/a7b9f2bf-7761-41f9-9c8e-ec6ef81b9d83" alt="Conditional formatting" width="100" height="150"><br/>

## Fixing inconsistensies 
Lastly, we'll address inconsistencies in letter casing such as 'AARON HERNANDEZ' and 'operations'  within the 'Name,' 'Department,' and 'Status' columns using '=PROPER()'.

<img src="https://github.com/user-attachments/assets/bc3cc525-529c-4ce6-a086-c604ee03c6d0" alt="Conditional formatting" width="300" height="150"><br/>

The dataset is now ready for further analysis.
