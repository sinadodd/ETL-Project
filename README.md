#  ETL Project Report
## Extract
Our data formats:
CSV, XLSX

Downloaded directly from:
- https://datacenter.kidscount.org/data#USA/2/0/char/0
- https://www.kff.org/

The raw data had more information than we wanted, including data for many years. We only wanted one year of data per factor, but chose to not care if we had the same year for all data. This could allow the most straightforward analysis by ranking the states.

## Transform
Data munging in Jupyter Notebook with Pandas. See the Jupyter Notebooks to reproduce the transformation process.

Mostly, this was wittling down the data to only what we needed. There was some datatype conversion and formatting so that percentages are in {:.1%} format.

## Load
We decided to use a relational database because the information we're gathering can be directly linked together. We have worked with MySQL and SQLITE in this course but chose SQLITE because we're working remotely/separately and its single-file storage format makes it easy to share.

See the Jupyter Notebooks to reproduce the SQLite database creation and loading.

Our final database has one table per parental factor and one table per child success indicator. All tables have a column for the state, and contain 1 year of data.


# Parental factors and their impact on child success indicators

## by Himani and Rosina

In a loose exploration of how assorted parenting inputs would affect assorted child success indicators, we have chosen to zero on in location (states) as a way to generalize and see if there might be any trends.

## CHILD SUCCESS INDICATORS - Himani

### Indicator:

### Indicator:

### Indicator:

#### Sources for child success indicators:


## PARENTAL FACTORS - Rosina

### Education:
- Children whose head-of-household has less than a high school degree

### Economic:
- Children in families on Public Assistance

### Cultural:
- Children in Immigrant Families

### Health:
- Children (<=17) without health insurance
- Breastfeeding, 2015

#### Sources for parental factors:
1. https://datacenter.kidscount.org/data#USA/2/0/char/0
2. https://www.kff.org/


