# COVID-data-analysis
Data taken from https://catalog.data.gov/dataset/covid-19-case-surveillance-public-use-data

## Columns in this Dataset

Column Name | Description | Type
------------ | ------------- | -------------
current_status | What is the current status of this person? "Laboratory-confirmed case Probable case" | Plain Text
cdc_report_dt | Date case was first reported to the CDC | Date & Time
sex | Sex "Male Female Unknown Other" | Plain Text
age_group | Age group "0 - 9 Years 10 - 19 Years 20 - 39 Years 40 - 49 Years 50 - 59 Years 60 - 69 Years 70 - 79 Years 80 + Years" | Plain Text
pos_spec_dt | Date of first positive specimen collection | Date & Time
hosp_yn | Was the patient hospitalized? | Plain Text
icu_yn | Was the patient admitted to an intensive care unit (ICU)? | Plain Text
death_yn | Did the patient die as a result of this illness? | Plain Text
medcond_yn | Pre-existing medical conditions? | Plain Text
onset_dt | Date of symptom onset | Date & Time

## Inference

* Except some, most of the columns contain categorial data. So let us try to derive as much as information with the available numerical and categorial data.

* Due to less numerical columns we cannot plot different types of plots like line, scatter and heat. So mostly we would be using histogram to identify the distribution of data.

## Data Analysis

Let us try to ask below questions and try to derive some insights from the available data. Check inside [Detailed Analysis](Analysis/COVID-data-analysis.md) for more detailed analysis on below questions.

1. Patients in which age group has been most affected ?

   Patients in the 50-59 age years group were most affected followed by 40-49 years and then 30-39 years.

2. Patients in which age group has most died due to this disease?

   Patients in 80+ years age group died mostly followed by 70-79 years.

3. Was pre-existing medical conditions increasing the chance of getting affected?

   We cannot arrive at a conclusion for those affected since there are many Unkown values but the death rate is more for those who had pre-existing medical conditions

4. Which age group was the first to know the symptoms?

   There is no age group which tops the list. The symptoms started to show from 1st January across various age group.

5. How many people who were probable cases died due to not being hospitalized?

   More people in high age group died than people in lesser age groups who were probable cases

6. How has the death rate varied as age increases?

   The death rate has increased considerably as age increases

7. What is the average time period between various stages (onset of symptom, specimen collection, reporting to CDC) of the disease?

   The time period between various stages in on a average of 5 days with total of 10 days.

8. Has the time between onset of symptom and death increased based on age? If so, which age group has the shortest time period to recover from onset of symptom?

   We cannot derive this analysis since we do not have the date of death for patients

9. What percentage of patients admitted to ICU actually recovered? Does this mean there is more possibility to recover if admitted to ICU?

   There are more who died in ICU than recovered. So there is no assurance that admission to ICU increases recovery rate

10. What portion of the patients who were not admitted to ICU died? Could the death rate be decreased if admitted to ICU?

    Those who died are less than those who recovered. Again admission to ICU does not guarantee recovery