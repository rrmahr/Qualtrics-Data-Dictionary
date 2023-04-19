# Qualtrics-Data-Dictionary
This code can be utilized to generate a data dictionary in csv format to accompany responses exported from the Qualtrics API.

Survey details including Variable Naming, recode values, and value labels can be exported using the Get Survey API from the Qualtrics API (documentation here: https://api.qualtrics.com/9d0928392673d-get-survey) if an account has API access. However, the export is in json format and requires additional processing to be easily legible and used to accompany survey responses, particularly when the data is categorical.

This code parses the data from the API export into a csv file at the survey response option level per survey question for several commonly used Qualtrics question types including the following information:
- Var_Name: variable / survey question name
- Var_Label: survey question text / description of variable
- Value: numeric answer choice value
- Value_Label: label for answer choice
- Data_Type: data type of variable (INT, FLOAT, STRING)
- Var_Order: order the question / variable appears in the survey
- Question_Type: type of question in Qualtrics

See a sample export here: https://github.com/rrmahr/Qualtrics-Data-Dictionary/blob/main/data_dictionary_export_example.csv

