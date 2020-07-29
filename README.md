# The Rural Uninsured: Driving Factors & Implications

## Introduction

According to recent census data, 8.8 percent of people in the United States do not have health insurance. That's 28 million people who may receive substandard medical care or be turned away due to their lack of status. Because the United States does not have nationalized healthcare, citizens rely on health insurance to cover medical expenses. There are a wide variety of coverage types offered by both private companies and public healthcare systems like Medicare and Medicaid. Rates of uninsured were at 18% before the Affordable Care Act (ACA) mandate in 2013. 

There are a myriad of factors that can lead to people being uninsured, including financial, historical, and cultural reasons. Firstly, insurance can be expensive, especially if you have high deductible plans that require you to spend a specific amount before insurance kicks in. Many people use these plans because they are cheaper if you don't often or intensly access medical care. However, if you do require expensive operations or tests, then the costs can quickly add up. Secondly, some people have cultural reasons for choosing to not have health insurance, such as an individualistic nature that resists a government mandate for universal health insurance. Thirdly, there are historical reasons both for and against, for example, slavery and discrimination in the South has led to an inequal distribution of wealth heavily skewed against Black populations. Looking at poverty rates in the United States, seven of the top ten poorest states are in the South. 

## The Problem

So why does this rate of uninsured matter? There is a personnal and societal component to answering this question. For the patient, being uninsured means that you may be turned away for your inability to pay or you may receive substandard medical care (fewer tests, less attention from the physician, etc). If the reason is severe, you may have to accumulate bad debt (knowingly using credit you will not be able to repay) to ensure you can access care. For the physician, you must balance the ethical implications of turning away patients for a lack of finances and the steps you may have to take to lessen their burden, for example, underwriting fees, exaggerating symptoms, or sending them to a publicly funded alternative. Societally, the uninsured place greater stress on our public health system, e.g. public clinics, and the safety nets in place to help them, mainly Medicare, Medicaid, or VA benefits.

## The Model

I have created a model that takes in **demographic features** (including rural/urban populations, poverty rates, and education level) and **community health indicators** (including the presence of community health centers and if the county is undersevered by medical infastructure). This linear regression model will allow us to comment on what features impact the rate of uninsured by county. 

### Data Collection & Cleaning

I concatenated four datasets for this project to flush out some of my hypothesized features. I started with a community health indicators set from [HealthData.gov](https://healthdata.gov/dataset/community-health-status-indicators-chsi-combat-obesity-heart-disease-and-cancer). Then I incorporated a few datasets from the Census Bureau to get median household income ([1](https://www.census.gov/topics/income-poverty/income/data/tables.html)), demographics ([2](https://data.world/exercises/linear-regression-exercise-1)), and rural vs urban breakdowns ([3](https://www.census.gov/programs-surveys/geography/guidance/geo-areas/urban-rural/2010-urban-rural.html)).

## Insights

## Future Directions

While an R<sup>2</sup> value of 0.39 is actually not bad for a social sciences project due to the difficulty in quantifying human decision making, there is obviously room for improvement. I would like to incorporate more granular data, for example, I suspect that household income would play a role in the rate of uninsured but because our data was limited to the county-level, counties with a mix of urban and rural populations could be influenced by the urban population's increased average income. 

There are also factors that could be affecting this rate that have been difficult to gather data on. I would propose a system of surveys and aggregating health records that could provide reasons as to why patients did not have insurance. For example, a list of health facilities with charity systems in place (where uninsured patients can access a general "fund" to pay for procedures) to examine how this affects the uninsured rate.