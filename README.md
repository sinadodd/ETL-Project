# Parental factors and their impact on child success indicators

## by Himani and Rosina

In a loose exploration of how assorted parenting inputs would affect assorted child success indicators, we have chosen to zero on in location (states) as a way to generalize and investigate if there might be any correlations.

#  ETL Project Report

## E - Extract

Our data was downloaded as:
CSV, XLSX

The raw data provided more information than we wanted, including data for many years. We only wanted one year of data per factor, but chose to not care if we had the same year for all data. When using the data in the future, this could allow for the most straightforward analysis by ranking the states.

## T - Transform

Data munging was performed in Jupyter Notebook with Pandas. See the the included Jupyter Notebooks to reproduce the transformation process.

Mostly, this was wittling down the data to only what we needed. There was some datatype conversion and formatting so that percentages are in {:.1%} format.

## L - Load

We decided to use a relational database because the information we're gathering can be directly linked together. We have worked with MySQL and SQLITE in this course but chose SQLITE because we're working remotely/separately and its single-file storage format makes it easy to share.

See the Jupyter Notebooks to reproduce the SQLite database creation and loading.

Our final database has one table per parental factor and one table per child success indicator. All tables have a column for the state, and contain 1 year of data.

# CHILD SUCCESS INDICATORS - Himani

### Indicator:
-

### Indicator:
-

### Indicator:
-

#### Sources for child success indicators:
1. https://datacenter.kidscount.org/data#USA/2/0/char/0


# PARENTAL FACTORS - Rosina

### Education:
- Children whose head-of-household has less than a high school degree (1)

### Economic:
- Children in families on Public Assistance (1) 

### Cultural:
- Children in Immigrant Families (1)

### Health:
- Children (<=17) without health insurance (1)
- Breastfeeding, 2015 (2)

#### Sources for parental factors:
1. https://datacenter.kidscount.org/data#USA/2/0/char/0
2. https://www.kff.org/womens-health-policy/state-indicator/breastfeeding-rates/?currentTimeframe=0&sortModel=%7B%22colId%22:%22Location%22,%22sort%22:%22asc%22%7D

