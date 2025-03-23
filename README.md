# Healthcare System Flu Shot Analysis 2022

## Project Background

The healthcare system provides primary and specialty care services across multiple counties, with a business model focused on patient-centered care, preventive health initiatives, and community outreach. Key business metrics include patient compliance rates, vaccination coverage, and demographic health equity. This project analyzes flu shot distribution in 2022 to identify trends, disparities, and opportunities for improving vaccination rates.

Insights and recommendations are provided on the following key areas:

- **Category 1:** Flu shot compliance by age group  
- **Category 2:** Flu shot compliance by race  
- **Category 3:** Geographic distribution of flu shots by county  
- **Category 4:** Temporal trends in flu shot administration  

The SQL queries used to inspect and clean the data for this analysis can be found [here](https://github.com/THoangPhuc03/Flu-Shot-Dashboard/blob/main/Flu_Shot.sql).  
  
An interactive Tableau dashboard used to report and explore flu shot trends can be found [here](https://public.tableau.com/views/FluShotDashboard_17418385495400/Dashboard1?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link).

You can find all the data i use [here](https://drive.google.com/drive/folders/1Tu5enmbM8ec0cuCufvfHg0_-j3XljNUy?usp=sharing)

## Data Structure & Initial Checks
The healthcare system’s main database structure consists of four tables: conditions, encounters, immunizations, and patients. A description of each table is as follows:
#### **1. conditions:**
- This table tracks diagnoses or conditions associated with patient encounters.
  
#### **2. encounters:** 
- This table logs healthcare visits and their associated costs.
  
#### **3. immunizations:
- This table is critical for tracking flu shot administration.
  
#### **4. patients:**
- This table provides demographic and geographic data for analysis.

![image](https://github.com/user-attachments/assets/f589cbed-ae73-48e6-94cb-ccaff5de9385)

---

## Executive Summary

### Overview of Findings

In 2022, the healthcare system achieved an overall flu shot compliance rate of 81.8%, administering 8,101 flu shots. Compliance varied significantly by age, race, and county, with the 18-34 age group showing the lowest compliance at 62.2%, and certain counties like Plymouth lagging behind. Temporal trends indicate a peak in flu shot administration during the fall months, aligning with flu season.

![Dashboard](https://github.com/user-attachments/assets/ffb96b4e-537c-48bb-9bfe-3a8e69af0535)

---

## Insights Deep Dive

### Category 1: Flu Shot Compliance by Age Group

- **Main Insight 1:** The 18-34 age group had the lowest compliance rate at 62.2%. This suggests a lack of engagement or awareness among younger adults, possibly due to perceived low risk of flu complications.  
- **Main Insight 2:** The 0-17 age group had the highest compliance rate at 94.9%. This is likely driven by pediatric vaccination programs and parental oversight.  
- **Main Insight 3:** The 65+ age group also showed high compliance at 91.2%, reflecting awareness of flu risks among older adults and targeted outreach efforts.  
- **Main Insight 4:** The 35-49 age group’s compliance rate of 68.8% indicates a moderate engagement level, potentially due to competing priorities like work and family responsibilities.  

![image](https://github.com/user-attachments/assets/b4954305-1148-487f-860b-917f1ac55c37)

### Category 2: Flu Shot Compliance by Race

- **Main Insight 1:** Native and Black populations had the highest compliance rates at 85.7% and 85.2%, respectively, indicating effective outreach to these groups.  
- **Main Insight 2:** The "Other" race category had the lowest compliance rate at 80.0%, suggesting potential gaps in targeting less-defined demographic groups.  
- **Main Insight 3:** White patients, who likely form a significant portion of the patient base, had a compliance rate of 81.3%, slightly below the overall average of 81.8%.  
- **Main Insight 4:** Asian and Hawaiian groups showed compliance rates of 82.6% and 82.9%, respectively, indicating relatively consistent vaccination uptake across these groups.  

![image](https://github.com/user-attachments/assets/1d731c34-7e32-4c30-9f0a-1f3d7e80535a)

### Category 3: Geographic Distribution of Flu Shots by County

- **Main Insight 1:** Plymouth County had the highest number of unvaccinated patients (80, Veronica McKenzie), indicating a need for targeted interventions in this area.  
- **Main Insight 2:** Suffolk County (Boston area) showed a high vaccination rate, likely due to better access to healthcare facilities and urban outreach programs.  
- **Main Insight 3:** Bristol County had a moderate number of unvaccinated patients (e.g., 52, Misty Upton), suggesting room for improvement in rural healthcare access.  
- **Main Insight 4:** The map highlights that counties like Essex and Middlesex have fewer unvaccinated patients, reflecting stronger vaccination efforts in these regions.  

![image](https://github.com/user-attachments/assets/bd6150fc-5489-49cb-89ea-ce9666970d8b)

### Category 4: Temporal Trends in Flu Shot Administration

- **Main Insight 1:** The running sum of flu shots shows a steep increase from September to November, peaking at around 8,000 shots, aligning with the start of flu season.  
- **Main Insight 2:** Flu shot administration was minimal from January to August, with a gradual increase starting in September, indicating seasonal vaccination patterns.  
- **Main Insight 3:** December saw a slight decline in new flu shots, suggesting that most patients who intended to get vaccinated did so earlier in the fall.  
- **Main Insight 4:** The cumulative total of 8,101 flu shots by year-end reflects a successful vaccination campaign, though late-season efforts could be improved.  

![image](https://github.com/user-attachments/assets/e9ed4982-63bc-4a6f-9e48-20c8b78c0dcd)

---

## Recommendations

Based on the insights and findings above, we would recommend the [public health team] to consider the following:  

- **Observation:** The 18-34 age group has the lowest compliance rate at 62.2%. **Recommendation:** Launch a digital marketing campaign targeting younger adults on social media platforms, emphasizing the importance of flu shots for community health.  
- **Observation:** The "Other" race category has the lowest compliance rate at 80.0%. **Recommendation:** Conduct focus groups to understand barriers for this demographic and tailor outreach programs accordingly.  
- **Observation:** Plymouth County has the highest number of unvaccinated patients. **Recommendation:** Increase mobile vaccination clinics in Plymouth County to improve access and awareness.  
- **Observation:** Flu shot administration peaks in the fall but drops in December. **Recommendation:** Extend vaccination drives into early winter with incentives like free health checkups to capture late adopters.  
- **Observation:** High compliance in the 0-17 and 65+ age groups. **Recommendation:** Leverage these groups as advocates to encourage vaccination among their peers and family members in lower-compliance age groups.  

---

## Assumptions and Caveats

Throughout the analysis, multiple assumptions were made to manage challenges with the data. These assumptions and caveats are noted below:  

- **Assumption 1:** Patients with missing race data were categorized as "Other," which may skew compliance rates for this group.  
- **Assumption 2:** County data was based on patient residence, but some patients may have received flu shots outside their home county, potentially affecting geographic trends.  
- **Assumption 3:** The vaccination records for December were incomplete due to reporting delays, so the running sum may underrepresent late-season shots.
