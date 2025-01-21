"""
README.md

# Housing Inequity 2008-2023 Exploratory Analysis

This document outlines the purpose and scope of the exploratory data analysis (EDA) conducted on the 2008-2023 housing data, with a specific focus on identifying and understanding housing inequities. This analysis is based on data from the **Public Use Database (PUDB)** provided by the Federal Housing Finance Agency (FHFA) and other relevant sources.

## Purpose

The primary goals of this exploratory analysis are to:

*   **Examine disparities in mortgage lending:** Identify and quantify differences in loan origination, denial rates, and loan types across various demographic groups, particularly focusing on racial and ethnic disparities.
*   **Analyze the impact of socio-economic factors on housing:** Investigate how factors such as income levels, location, and the type of loan (conventional vs. non-conventional) affect access to homeownership and mortgage terms.
*   **Explore geographic patterns of housing inequities**: Use census tract-level data to examine how housing disparities vary across different neighborhoods and regions.
*   **Assess the role of loan types and lender:** Evaluate disparities in the types of loans (e.g., FHA-insured vs conventional) and how they relate to race and ethnicity of the borrowers.
*   **Inform policy and intervention strategies:** Provide insights that can be used to develop targeted interventions and policies aimed at reducing housing inequities and promoting fair access to homeownership.
*   **Understand the impact of climate risk:** Explore how climate-related factors intersect with existing housing inequities.

## Data Sources

This analysis utilizes data from the following sources:

*   **FHFA Public Use Database (PUDB):**
    *   **Single-Family Mortgage-Level Owner-Occupied 1-Unit Properties (National File A):** [1]
        *   Provides mortgage-level data for owner-occupied 1-unit properties.
    *   **Single-Family Unit-Level Properties (1-4), includes Renter-Occupied 1-Unit Properties (National File B):** [1]
        *   Contains unit-level data for properties with 1-4 units, including renter-occupied 1-unit properties.
    *   **Single-Family Census Tract Files from Freddie Mac and Fannie Mae:** [1]
         * Provides detailed geographic information for single-family properties.
        *   Combined GSE File available.
    *   **Multifamily National File:** [1]
         *   Includes data on all multifamily properties by unit and mortgages.
    *   **Multifamily Census Tract File:** [1]
        *   Provides geographic information for multifamily properties.
    *   **FHLBank Public Use Database**: [1]
        *   This dataset contains census tract-level data related to mortgages purchased by each Federal Home Loan Bank.
    *   These datasets provide detailed information about mortgage acquisitions, including loan characteristics, borrower demographics, and property information.
*  **2023 Low-Income Areas File**:
    * This file establishes low-income area designations for census tracts which are used for scoring mortgage purchases toward the single-family housing goals for Fannie Mae, Freddie Mac, and the Federal Home Loan Banks.
    * The FHFA website is the source [1].
*   **Home Mortgage Disclosure Act (HMDA) data:**
    *   Used for analyzing loan applications and originations by race and ethnicity.
    *   The Consumer Financial Protection Bureau is a source of HMDA data.
*   **US Census Bureau, American Community Survey (ACS) data:**
    *   Used for calculations based on census data.
    *   Available at the US Census Bureau website.

## Key Areas of Investigation

The analysis will focus on several key areas:

*   **Loan Application and Origination Disparities**:
    *   Comparing the volume and approval rates of loan applications for different demographic groups, particularly Black and White applicants.
    *   Analyzing the types of loans originated (conventional vs. non-conventional) for different demographics and evaluating approval rates.
    *   Assessing loan denial rates for various demographic groups and exploring the reasons behind these denials.
*   **Socioeconomic Factors and Mortgage Access:**
    *   Examining the relationship between income levels and mortgage approval rates.
    *   Analyzing how loan-to-value ratios, debt-to-income ratios, and affordability impact access to mortgages.
    *   Investigating the effects of low-income area designations and minority tract status on mortgage lending.
*   **Geographic Disparities:**
    *   Identifying areas with high denial rates based on location, particularly areas with high percentages of minority residents.
    *   Exploring correlations between climate-related risks and areas with high concentrations of Black homeownership.
*   **Climate and Environmental Risk:**
    *   Analyzing the intersection between climate change and homeownership, particularly for Black communities.
    *  Evaluating how factors such as flood risk and historical redlining practices influence housing affordability and access.

## Methodology

The analysis will involve a combination of quantitative methods, including:

*   Descriptive statistics to summarize key variables.
*   Comparative analysis to identify disparities across different demographic and geographic groups.
*   Correlation analysis to examine relationships between variables such as income, loan type, location, and denial rates.
*   Data visualizations (e.g., charts, maps) to present the findings clearly and effectively.
*   Utilizing python libraries such as pandas, NumPy, Seaborn, and Matplotlib.

## Expected Outcomes

This exploratory analysis is expected to provide:

*   A clear understanding of housing inequities in 2023.
*   Identification of key factors contributing to these inequities.
*   Data-driven insights for developing targeted policies and interventions.
*   A foundation for more in-depth research and analysis.

## How to Use This Analysis

The findings from this analysis will be used to:

*   Inform community outreach and education efforts.
*   Guide the development of fair housing policies.
*   Support advocacy efforts to promote housing equity.
*   Raise awareness about the systemic issues contributing to housing inequities.

## Next Steps

*   Data cleaning and preprocessing.
*   Exploratory analysis of key variables.
*   Statistical analysis to identify significant patterns and relationships.
*   Visualization of results to communicate findings.

## This analysis is a crucial step towards ensuring fair and equitable housing opportunities for all.

# Here's a list of the cited documents, websites, and datasets mentioned in the README
*   Public Use Database (PUDB) datasets:

x*  Single-Family Mortgage-Level Owner-Occupied 1-Unit Properties (National File A)

*  Single-Family Unit-Level Properties (1-4), includes Renter-Occupied 1-Unit Properties (National File B)

*  Single-Family Census Tract Files from Freddie Mac and Fannie Mae

*  Multifamily National File

*  Multifamily Census Tract File

*  FHLBank Public Use Database

*  2023 Low-Income Areas File [This file is mentioned as being sourced from the FHFA website.]
Websites:

*  Federal Housing Finance Agency (FHFA) website: This is the primary source for the PUDB datasets, the Low-Income Area file, and other information related to housing finance.

*  Consumer Financial Protection Bureau: This is a source for Home Mortgage Disclosure Act (HMDA) data [Not directly cited but understood to be the source]

*  US Census Bureau website: This is a source for the American Community Survey (ACS) data [Not directly cited but understood to be the source]
Datasets:

*  Home Mortgage Disclosure Act (HMDA) data: Data used for analyzing loan applications and originations by race and ethnicity.

*  American Community Survey (ACS) data: Census data used for socio-economic calculations.

*  MNIST digits dataset: A dataset containing 60,000 examples of handwritten digits 0 through 9 that are grayscale images of size 28x28 and is used as a recurring example in the sources.

*  California Housing Prices dataset: A dataset based on the 1990 California census used as an example for machine learning applications.

*  TREX (T-Rex) dataset: A dataset consisting of Knowledge Base Triples (KBTs) extracted from Wikipedia.

*  WikiText2 dataset: A HuggingFace dataset that contains prompts used in general text generation.

*  RealToxicityPrompts: A dataset that evaluates toxicity by attempting to get a model to generate toxic language.

*  Gigaword dataset: A dataset consisting of news article headlines, used in text summarization tasks.

*  BoolQ dataset: A dataset consisting of yes/no question and answer pairs.

*  NaturalQuestions dataset: A dataset consisting of real user questions submitted to Google search.

*  TriviaQA dataset: A dataset containing over 650K question-answer-evidence-triples, used in question and answer tasks.

*  Women's E-Commerce Clothing Reviews dataset: A dataset that contains clothing reviews written by customers, used in text classification tasks.
## Additional Notes:

*  The PUDB datasets are released annually by the FHFA.

*  The single-family datasets include loan-level records that contain data on income, race, and gender of each borrower, as well as the census tract location of the property, loan-to-value (LTV) ratio, and other related data.

*  The multifamily datasets include information on the unpaid principal balance and type of seller/servicer.

*  The FHLBank PUDB contains census tract level data relating to mortgages purchased by each Federal Home Loan Bank.

The files from the FHLBanks are unaudited and are reported directly by the Federal Home Loan Banks to the FHFA.
