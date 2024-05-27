# Emergency Room Visit Report

## Overview

The Emergency Room Visit Report project aims to provide comprehensive insights into the visits to the emergency room. This project utilizes various metrics and visualizations to offer a detailed analysis of patient visits, appointments, and satisfaction levels, segmented by different demographics and time periods.

## Key Metrics

- **Total Patients**: The total number of patients who visited the emergency room.
- **Administrative Appointments**: The number of appointments scheduled for administrative purposes.
- **Non-Administrative Appointment Percentage**: The percentage of appointments that are non-administrative.
- **Average Satisfaction Score (Not Rated 3)**: The average satisfaction score of patients, excluding those who rated the service as 3.
- **Average Wait Time**: The average time patients wait before receiving service.
- **Referral Patients**: The number of patients referred by other healthcare providers.
- **Walk-In Patients**: The number of patients who arrived at the emergency room without a prior appointment.

## Slicers

- **Time**: Allows filtering of data based on specific time periods.

## Visualizations

1. **Patients by Week Type**: Displays the distribution of patients across different types of weeks (e.g., weekdays vs. weekends).
2. **Patients by Age Group**: Segments patient data by various age groups.
3. **Total Patient Visits by Year**: Shows the trend of total patient visits over the years.
4. **Patients by Department Referral**: Highlights the number of patients referred by different departments.
5. **Total Patients by Month**: Illustrates the monthly trends in patient visits.
6. **Gender Breakdown**: Provides a gender-wise distribution of patient visits.
7. **Average Satisfaction Score and Average Wait Time by Age Group and Patient Race**: Shows the average satisfaction scores and wait times, segmented by age groups and race.

## How to Use

1. **Open the Report**: Access the report through your preferred BI tool.
2. **Select Slicers**: Use the time slicers to filter the data for specific periods.
3. **Analyze Visualizations**: Review the various visualizations to gain insights into different aspects of emergency room visits.
4. **Interactivity**: Click on different segments of the charts to drill down into more detailed data.

## Data Source

The data for this report is sourced from the hospital's emergency room database, which includes records of patient visits, appointments, satisfaction surveys, and referral details.

## Learnings

### DAX Functions

- **Max and Min Highlighting**: We used DAX to identify and highlight the months with the highest and lowest number of patient visits. This involved creating a variable to summarize monthly patient data and then using `MINX` and `MAXX` functions to find the minimum and maximum values.

- **SWITCH Function**: The `SWITCH` function was essential for returning specific values based on conditions. It allowed us to create a dynamic measure that highlights the maximum and minimum values directly in the visualizations.

- **CALCULATE Function**: The `CALCULATE` function was extensively used to modify the context of calculations. For instance, calculating the total patient visits for the current month while ignoring other filters ensured accurate comparison with the minimum and maximum values.

### Sparklines

- **Sparklines**: We incorporated sparklines to provide a quick, visual representation of data trends over time. Sparklines helped in showing trends in patient visits, average satisfaction scores, and wait times across different time periods without taking up much space.

## Conclusion

The Emergency Room Visit Report provides a detailed and insightful analysis of patient visits to the emergency room. By leveraging key metrics and advanced visualizations, this report helps in understanding the dynamics of patient flow, satisfaction levels, and appointment types. The use of DAX functions like `SWITCH`, `CALCULATE`, and context evaluation techniques such as `REMOVEFILTERS` ensured accurate and meaningful data representation. Sparklines added a valuable visual dimension to the report, allowing for quick trend analysis.

Overall, this project demonstrates the power of data analytics in healthcare, offering actionable insights that can lead to improved patient care and operational efficiency. By understanding patterns in patient visits and satisfaction, hospital administrators can make informed decisions to enhance the quality of emergency room services. This report serves as a valuable tool for continuous monitoring and improvement of emergency room operations.



By following the above structure, users can effectively navigate and utilize the Emergency Room Visit Report to gain meaningful insights into patient visits and other related metrics.
