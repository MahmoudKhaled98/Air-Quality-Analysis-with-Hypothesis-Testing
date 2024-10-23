# Air Quality Analysis with Hypothesis Testing

## Project Overview

This project focuses on analyzing the **Air Quality Index (AQI)** across various U.S. regions, particularly targeting areas relevant to the environmental think tank **Repair Our Air (ROA)**. The AQI serves as a critical measure of air quality, where values closer to 0 indicate minimal health risks, while higher values pose increasing public health concerns. ROA is formulating policy recommendations to improve air quality, and this analysis aims to assess the potential impact of these policies based on AQI data.

The dataset includes AQI values from multiple counties and states, facilitating an exploration of the mean AQI and hypothesis testing to understand differences in air quality across regions.

## Table of Contents

- [Introduction](#introduction)
- [Tools Used](#tools-used)
- [Project Structure](#project-structure)
- [Data Exploration and Statistical Analysis](#data-exploration-and-statistical-analysis)
  - [Step 1: Imports](#step-1-imports)
  - [Step 2: Data Exploration](#step-2-data-exploration)
  - [Step 3: Statistical Analysis](#step-3-statistical-analysis)
  - [Step 4: Results and Evaluation](#step-4-results-and-evaluation)
- [Key Insights](#key-insights)
- [Conclusion](#conclusion)
- [How to Run](#how-to-run)
- [References](#references)

## Introduction

Air quality is a vital environmental health indicator, significantly influencing public health and policy decisions. In this project, I analyze AQI data to evaluate specific hypotheses related to air quality in various regions, focusing on:

1. ROA is considering a metropolitan-focused approach. Within California, they want to know if the mean AQI in Los Angeles County is statistically different from the rest of California.
2. With limited resources, ROA has to choose between New York and Ohio for their next regional office. Does New York have a lower AQI than Ohio?
3. A new policy will affect those states with a mean AQI of 10 or greater. Will Michigan be affected by this new policy?

Key objectives include:
- Conducting hypothesis tests to evaluate AQI differences.
- Drawing insights that can inform ROA's policy recommendations.

## Tools Used

- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations.
- **SciPy**: For statistical functions and hypothesis testing.

## Project Structure

The project is organized into four main steps:
- **Step 1: Imports**: Importing necessary libraries for analysis.
- **Step 2: Data Exploration**: Exploring the dataset's structure and generating descriptive statistics.
- **Step 3: Statistical Analysis**: Conducting hypothesis tests and visualizing results.
- **Step 4: Results and Evaluation**: Presenting findings and discussing their implications for air quality policy.

## Data Exploration and Statistical Analysis

### Step 1: Imports
The required libraries are imported to facilitate data manipulation, visualization, and statistical analysis.

### Step 2: Data Exploration
I load and explore the dataset to understand its structure and the characteristics of the AQI values. Key questions addressed include:
- What does the AQI data represent?
- What are the descriptive statistics, including mean and count?
- Are there any missing values in the AQI data?

### Step 3: Statistical Analysis
I formulate and test the following hypotheses:
1. **Los Angeles County vs. Rest of California**:
   - $H_0$: No difference in mean AQI.
   - $H_A$: Significant difference in mean AQI.
   - **P-value**: 0.04983 (Reject $H_0$; support for metropolitan-focused strategy).

2. **New York vs. Ohio**:
   - $H_0$: New York's mean AQI ≥ Ohio's mean AQI.
   - $H_A$: New York's mean AQI < Ohio's mean AQI.
   - **P-value**: 0.030 (Reject $H_0$; New York has lower mean AQI).

3. **Michigan's AQI**:
   - $H_0$: Michigan's mean AQI ≤ 10.
   - $H_A$: Michigan's mean AQI > 10.
   - **P-value**: 0.940 (Fail to reject $H_0$; unlikely to be affected by the new policy).

### Step 4: Results and Evaluation
I present visualizations of the AQI distributions and evaluate the results of the hypothesis tests, discussing their implications for ROA's policy decisions.

## Key Insights

- **Statistical Significance of AQI Levels**: The analysis revealed that the mean AQI for Los Angeles is statistically different from the mean AQI across the rest of California at a 5% significance level, indicating significant air quality concerns specific to Los Angeles.

- **Comparative Analysis Between States**: The findings demonstrated that New York has a lower mean AQI compared to Ohio, suggesting better air quality in New York, which may inform public health strategies and resource allocation.

- **Limitations in Conclusions**: The analysis was unable to establish, at the 5% significance level, that Michigan's mean AQI exceeds a value of 10. This uncertainty highlights a need for further investigation and potentially larger sample sizes to draw more definitive conclusions.

- **Importance of Statistical Context**: Presenting the null and alternative hypotheses for each test, along with the p-values and types of tests conducted, provides stakeholders with essential context to understand the implications of the findings and their significance in air quality management.

## Conclusion

This project highlights the importance of hypothesis testing in environmental data analysis. By evaluating AQI levels across various regions, I provide actionable insights for ROA's policy recommendations aimed at improving air quality. The findings underscore the role of statistical analysis in guiding effective environmental policies.

## How to Run

1. **Clone the repository**:

    ```bash
    git clone <https://github.com/MahmoudKhaled98/Air-Quality-Analysis-with-Hypothesis-Testing.git>
    ```

2. **Install the required dependencies**:

    ```bash
    pip install -r requirements.txt
    ```

3. **Run the Jupyter notebook**:

    ```bash
    jupyter notebook
    ```

## References

- [Pandas Documentation](https://pandas.pydata.org/)
- [NumPy Documentation](https://numpy.org/)
- [SciPy Documentation](https://scipy.org/)
