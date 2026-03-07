# Malaga Tourist Rental Market Analysis

Academic project focused on the statistical analysis of the tourist rental market in Málaga, with a business-oriented approach to pricing, demand behavior, market positioning, future occupancy, and cancellation impact.

## Project objective

The goal of this project is to analyze the performance of a tourist apartment portfolio in Málaga and compare it with the local market using descriptive and inferential statistics.

The analysis is designed to answer business-related questions such as:

- What are the main demand patterns in the portfolio?
- How are ADR, booking lead time, and length of stay distributed?
- How is the portfolio positioned against the Málaga market in terms of pricing?
- What is the estimated market occupancy for the next 60 days?
- What is the expected revenue impact of cancellations?

## Data sources

This project is based on two datasets:

1. Historical booking data from an internal apartment portfolio
2. Market data obtained from Airbnb listings in Málaga

The original datasets are **not included in this repository due to confidentiality restrictions**.  
This project is shared for portfolio purposes and focuses on methodology, analysis workflow, and conclusions.

## Tools used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Folium

## Methodology

The project includes:

- Data cleaning and preprocessing
- Variable transformation and standardization
- Outlier treatment
- Descriptive statistical analysis
- Data visualization
- Normality testing (Shapiro-Wilk)
- QQ plots
- Mean comparison tests
- Log transformations
- Confidence intervals and proportion estimation

## Main analyses

### 1. Market structure in Málaga
Analysis of the tourist rental market in Málaga, including:

- Supply size
- Capacity distribution
- Price distribution
- Market asymmetry
- Estimated future occupancy
- Geographic distribution of listings

### 2. Portfolio demand analysis
Study of key business variables such as:

- ADR (Average Daily Rate)
- Booking lead time
- Length of stay
- Cancellation rate

### 3. Competitive pricing comparison
Comparison between the portfolio and the Málaga market using average price per guest and statistical testing.

### 4. Future occupancy estimation
Approximation of market occupancy over the next 60 days based on listing availability.

### 5. Cancellation impact estimation
Estimation of the expected revenue loss associated with cancellations using historical portfolio data.

## Key takeaways

- The Málaga tourist rental market shows a broad and heterogeneous structure, with a concentration in mid-range pricing and a premium upper tail.
- Key variables such as ADR, lead time, and length of stay do not follow a normal distribution.
- After adjusting for capacity, the portfolio shows a competitive market positioning in pricing terms.
- Future occupancy and cancellation behavior can be used as valuable inputs for revenue and operational decision-making.

## Repository structure

```text
malaga-tourist-rental-market-analysis/
├── notebook.ipynb
├── README.md
├── data-not-included.txt
└── images/

## Confidentiality note

The original CSV files are not published in this repository because they contain confidential or restricted-use data.

This repository is intended to showcase:

analytical approach,

statistical methodology,

data cleaning and transformation skills,

and business-oriented interpretation of results.

**Author**

**Juan Sanchez**
Business Analytics | Revenue | Operations | BI