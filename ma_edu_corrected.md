# Massachusetts Education System Analysis: Beyond Class Size
![ma_edu_title photo](https://github.com/user-attachments/assets/3e320740-884b-4645-b64f-43579014e5c8)

## Project Background
The Massachusetts Department of Education has been operating since 1789. As of 2017, the system serves nearly one million students across 1,861 schools, making it one of the largest public education systems in the United States. The department's primary focus is on providing quality education while managing resources effectively and ensuring equitable outcomes for all students.

Key business metrics include:
* Graduation rates
* College admission rates  
* Academic performance (particularly in math)
* Student-to-teacher ratios
* Economic status of student populations

An interactive Tableau dashboard used to report and explore sales trends can be found here


## Data Structure & Initial Checks
The dataset consists of 1,861 rows and 302 columns, containing comprehensive information about Massachusetts schools.

![Screenshot 2025-01-27 175652](https://github.com/user-attachments/assets/a0b3dd7f-fc51-4fd7-9a4c-de314e31846f)

While the diagram isn't comprehensive, it captures the main data points used for focus of this project and its logical grouping:
* School Demographics
* Academic Performance 
* Resource Allocation
* Student Services

Worth Noting:
* A: Advanced performance level
* P+A: Proficient and Advanced combined
* NI: Needs Improvement
* CPI: Composite Performance Index (scale from 0-100 that measures progress toward proficiency)

## Executive Summary 

### Overview of Findings
Analysis of Massachusetts education data reveals that traditional assumptions about educational success factors may need reassessment. Surprisingly, larger class sizes often correlate with higher college attendance rates, suggesting that socioeconomic factors may have more impact than class size alone. The data shows significant disparities in graduation rates, with specialized schools like Curtis-Tufts requiring different success metrics due to their unique student populations. Top-performing districts like Hingham, Winchester, and Lynnfield demonstrate excellence in math despite varying economic conditions.

![data corrections](https://github.com/user-attachments/assets/47217948-a451-43e7-9e18-4916e9cbd0f2)

### Insights Deep Dive

#### Category 1: Student Demographics and Performance
* Specialized schools require unique metrics
  * Curtis-Tufts School's 0% graduation rate reflects its focus on students with disabilities
  * Traditional metrics may not capture important developmental outcomes
  * 100% of student body classified as Students With Disabilities
    
![grad pct](https://github.com/user-attachments/assets/c18cb713-5b77-4bd4-92c9-482cc455ccff)

#### Category 2: Resource Allocation and Outcomes
* Class size findings challenge conventional wisdom
  * Larger class sizes correlate with higher college attendance rates
  * R-squared value of 0.19 indicates statistical significance (p < .05)
  * Class size explains 19% of graduation rate variation
* Economic status significantly impacts outcomes
  * Schools with higher percentages of economically disadvantaged students show lower college attendance rates
  * Exception: "The Gateway to College" achieves 100% college attendance despite 30% economically disadvantaged population

![college attendance vs class size](https://github.com/user-attachments/assets/4157f216-4e09-4b0c-9e08-b615f9dd0295)


#### Category 3: District Performance
* Top-performing districts in mathematics
  * Hingham (91%)
  * Winchester
  * Lynnfield 
* Success achieved despite varying economic conditions
  
![econ disadvtg vs grad rate](https://github.com/user-attachments/assets/87197c83-4d06-409e-ab49-1c394cfb212b)

#### Category 4: Access and Equity
* Economic disparities
  * Clear pattern of lower college attendance rates in economically disadvantaged areas
  * Some schools successfully overcome these challenges
  * Need for targeted support in struggling districts
 
![collegeattend vs econ](https://github.com/user-attachments/assets/8eb8a11b-07d2-4573-85ab-6f98ae669b6a)


## Recommendations
Based on the insights above, we recommend the following actions:

* Reevaluate resource allocation strategies
  * Focus on socioeconomic support rather than exclusively reducing class sizes
  * Implement successful practices from schools like "The Gateway to College"
* Develop specialized success metrics
  * Create alternative performance measures for specialized schools like Curtis-Tufts
  * Include developmental and life-skills outcomes in evaluation criteria
* Target economic support programs
  * Identify and support schools with high percentages of economically disadvantaged students
  * Study and replicate successful programs from high-performing schools with challenging demographics
* Enhance district-level support
  * Study and document best practices from top-performing districts
  * Develop mentorship programs between high and low-performing districts
* Implement data-driven decision making
  * Continue detailed analysis of factors affecting student success
  * Establish regular monitoring of key performance indicators

## Assumptions and Caveats

### Graduation Rate Interpretation
* Traditional graduation rates may not reflect success for specialized schools
* Alternative success metrics may be more appropriate for certain student populations such as College Attendance rate

### Statistical Significance
* Class size correlation with college attendance (R-squared = 0.19) assumes linear relationship
* Other factors may account for remaining 81% of variation

### Data Completeness
* Analysis based on available data points
* Some schools may have incomplete or missing data, given that the highest grade here is 10th grade, suggesting data for 11th and 12th grade are missing

## Future Directions
* Investigate characteristics of schools below 20% graduation rate
* Analyze impact of additional factors such as:
  * Race
  * SAT participation
  * School funding
  * Teacher salaries
* Develop more comprehensive success metrics for specialized schools
