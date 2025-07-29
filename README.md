#  Job Role Skill Match Analyzer

## Table of Contents
- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Data Analysis](#data-analysis)
- [Results](#results)
- [References](#references)

### Project Overview
This project is a Python-based data analytics tool designed to analyze various job roles and evaluate how well a candidate's skills align with industry demands. 
The code simulates a real-world scenario where a job seeker filters job roles related to "Data Analyst" and checks skill compatibility using structured Python classes and logic.

#### Time Series Chart
![Untitled](https://github.com/user-attachments/assets/a73952e5-92fb-41b3-9f7b-daefb44d4983)


#### Cluster Bar Chart
![Untitled1](https://github.com/user-attachments/assets/4f89bb26-ae74-462d-b7e5-2055a67a372a)


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
