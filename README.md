# Tableau Emergency Room dashboard

A brief description of what this project does and who it's for

# PROBLEM STATEMENT

### Dashboard Link: https://public.tableau.com/app/profile/tumisang.maramane/viz/HospitalEmergencyRoomVisits_17072236482160/Dashboard1?publish=yes

## Problem Statement

The emergency department (ER) of a hospital aims to provide efficient and effective care to patients in need of urgent medical attention. However, managing and analysing the influx of patients, their demographics, satisfaction levels, and department referrals can be challenging without a centralised system for data visualisation and analysis. To address this challenge, there is a need to develop a Tableau dashboard that provides comprehensive insights into ER operations, including patient volume trends, demographic distribution, satisfaction scores, average wait times, and department referrals. This dashboard will enable hospital administrators, healthcare providers, and decision-makers to make informed decisions, optimise resource allocation, and enhance the overall quality of care provided in the emergency department


### Steps followed 
### 1. Data Connection and Structure Understanding:

- Connect to the "Hospital ER" data source in Tableau.
- Examine the fields available in the dataset, including patient ID, satisfaction scores, department referrals, patient demographics (such as age and gender), and timestamps for ER visits.
- Data was cleaned with mySQL workbench so all null values and dates were fixed and abbreviated. 

### Age Grouping Calculation: 

Create a calculated field called "Age Groupings" to categorise patients into different age groups.
Formula:

IF [Patient Age] >= 0 and [Patient Age]<= 18 then ‘0-18'

ELSEIF [Patient Age] >= 19 and [Patient Age]<= 65 then ’19-65'

ELSEIF [Patient Age] >= 66 THEN '66+'
END

Use conditional logic in the calculated field to assign patients to age groups based on their ages (0-18, 19-65, 66+).

![Age Grouping](https://github.com/TumiSpaces/Tableau-Hospital-Emergency-Room-Visits/assets/124736182/453d937a-9219-4e2e-9daa-ac8a79fcaa7e)

### Visulaization Creation 

- Build various visualisations to analyse ER metrics:
- Tree Map showing the number of patients visiting the ER over time.
- Line chart illustrating patient satisfaction scores over time.
- Line chart or bar chart depicting the average wait time for patients.
- Bar chart chart representing patient race.
- Bar chart showcasing department referrals.

Average wait time 
![wait time](https://github.com/TumiSpaces/Tableau-Hospital-Emergency-Room-Visits/assets/124736182/57e848cf-508b-4941-a139-8a8b62dd32fe)

Visiting time
![Visiting time](https://github.com/TumiSpaces/Tableau-Hospital-Emergency-Room-Visits/assets/124736182/cfd11d49-b369-4a8a-aae4-4202a1e4c3e1)

### Dashboard Layout

- Create a dashboard layout with distinct sections for each visualisation.
- Utilise horizontal containers to organise and group related visualisations together.
- Adjust the size and alignment of visual elements within each section for consistency and aesthetics.
- Remove unnecessary grid lines and background colours to keep the dashboard clean and focused.
- Ensure that each section of the dashboard is clearly labeled and easily navigable.

### Tooltip Standatdisation

- Standardise tooltips across visualisations to provide consistent and informative details.
- Update tooltips to use descriptive language and relevant metrics (e.g., "Patient volume" instead of "count of patient ID").
Ensure tooltips are clear, concise, and provide valuable insights to users when they hover over visual elements.

### Final Touches and Polish

Add visual elements such as icons or images to enhance the dashboard's visual appeal and clarity.
Align text and adjust font sizes to maintain consistency and readability throughout the dashboard.
Use colour schemes and formatting techniques to highlight important information and guide the user's attention.
Apply inner and outer padding to create spacing between visual elements and improve overall layout aesthetics.

### Experimentation and Customisation

Encourage experimentation with different chart types, colours, and layouts to find the most effective way to present data.

Customise the dashboard based on specific requirements and preferences, such as branding guidelines or user preferences.
Continuously iterate and refine the dashboard based on user feedback and evolving data needs to ensure its effectiveness and relevance over time.
By following these elaborated steps, you can create a comprehensive and visually appealing Tableau Emergency Room dashboard that effectively communicates key metrics and insights to users

## INSIGHT DRAWN 


Patient Volume Trends: 

The dashboard reveals fluctuations in the number of patients visiting the emergency department over time. This insight can help hospital administrators anticipate peak periods and allocate resources accordingly to ensure efficient patient flow and minimise wait times.

Demographic Distribution:

Analysis of patient demographics, including gender and age groups, provides valuable insights into the composition of the patient population accessing emergency services. Understanding demographic trends can aid in tailoring healthcare services to meet the specific needs of different patient groups.

Patient Satisfaction Scores:
 
Monitoring patient satisfaction scores over time allows healthcare providers to gauge the quality of care provided in the emergency department. Identifying trends in satisfaction levels can highlight areas for improvement and guide efforts to enhance the overall patient experience.
![SATISFACTION](https://github.com/TumiSpaces/Tableau-Hospital-Emergency-Room-Visits/assets/124736182/95c2af1b-2028-4672-b1bc-d75b750c89dc)

Average Wait Times: 

Tracking average wait times for patients seeking emergency care helps identify bottlenecks in the triage and treatment process. By reducing wait times, hospitals can improve patient outcomes and satisfaction while maximising the efficiency of emergency department operations.

Department Referrals:

 Analysis of department referrals provides insights into the types of medical conditions and services required by patients accessing the emergency department. Understanding referral patterns can inform resource allocation and facilitate collaboration between different hospital departments to streamline patient care pathways.

![dept](https://github.com/TumiSpaces/Tableau-Hospital-Emergency-Room-Visits/assets/124736182/1174181b-050a-47b0-bea3-d4d6980523f5)

Busiest Times in the ER: 

The heat map visualisation highlights the busiest times in the emergency department, enabling administrators to optimise staffing levels and resource allocation during peak periods to ensure timely and effective patient care.

Patient Visits by Race: 

Examining patient visits by race can help healthcare providers identify disparities in access to emergency services and tailor interventions to address healthcare equity issues.

![RACE](https://github.com/TumiSpaces/Tableau-Hospital-Emergency-Room-Visits/assets/124736182/57f9e2c3-cf8a-47f0-9744-8ee6ff306208)


Overall Performance Metrics:
 
 By aggregating key performance metrics, such as average wait times and patient satisfaction scores, hospital administrators can assess the overall effectiveness and efficiency of emergency department operations and identify opportunities for improvement.

These insights derived from the Tableau Emergency Room dashboard empower healthcare providers and decision-makers to make data-driven decisions aimed at enhancing patient care, optimising resource allocation, and improving operational efficiency in the emergency department
![DASHBOARD](https://github.com/TumiSpaces/Tableau-Hospital-Emergency-Room-Visits/assets/124736182/a528fabc-4921-4d28-b1e7-4bec4bd5b006)

