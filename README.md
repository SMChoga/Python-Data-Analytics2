#  Job Role Skill Match Analyzer

## Table of Contents
- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Analysis](#data-analysis)
- [Results](#results)
- [References](#references)

### Project Overview
This project is a Python-based data analytics tool designed to analyze various job roles and evaluate how well a candidate's skills align with industry demands. 
The code simulates a real-world scenario where a job seeker filters job roles related to "Data Analyst" and checks skill compatibility using structured Python classes and logic.

#### Time Series Chart
<img width="1308" height="725" alt="1" src="https://github.com/user-attachments/assets/fa0faa73-c618-497c-b869-f935ad2a976a" />



#### Cluster Bar Chart
<img width="1366" height="768" alt="2" src="https://github.com/user-attachments/assets/e5bcc367-4a72-47ee-9d5a-d51a783770ef" />


### Data Source
- data_jobs.csv

### Tools
Python for data analysis


### Data Analysis
Include interesting code/features worked with
```python

##### Class and Objects 

job_title = 'Data Analyst'
job_location = 'United States'
job_salary = 90000
class JobPost:
    def __init__(self, title, location, salary):
        self.title = title
        self.location = location
        self.salary = salary
    
job_1 = JobPost(job_title, job_location, job_salary)
job_1.title
'Data Analyst'

##### Function
job_requirement = 'SQL'
application_skill = 'Excel'
experience = 7

if application_skill == job_requirement:
    print('Skilled')
elif application_skill == 'python':
    print ('skilled')
elif experience > 10:
    print ('Experienced','and', 'Skilled')
else:
    print('No Experience', 'and ', 'No Skill')

list(filter(lambda job: job['remote'] and 'Python' in job['job_skills'], jobs_data))
```

### Results
The analysis results are summarized as follows:
- The tool successfully extracted job roles that contain the term "Data Analyst" from a list of 50+ roles.
- It identified which roles matched the candidate’s skillset, helping determine if the applicant qualifies for the position.
-The approach highlighted that the candidate matched well with roles like Data Analyst, Business Intelligence Analyst,
  and partially with others that required additional tools like R, Tableau, or TensorFlow.

### References
[Luke Barousse - YouTube Channel](https://www.youtube.com/watch?v=wUSDVGivd-8&list=PL9PrwgRNlv62OiqVlASto1N4cAQRg60dr&index=19&pp=gAQBiAQB)
