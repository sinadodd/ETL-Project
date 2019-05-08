# ETL Project: Parental factors and their impact on child success indicators

## by Himani and Rosina

In a loose exploration of how assorted parenting inputs would affect assorted child success indicators, we have chosen to zero on in location (states) as a way to generalize and see if there might be any trends.

## CHILD SUCCESS INDICATORS - Himani

### Indicator:

### Indicator:

### Indicator:

#### Sources for child success indicators:


## PARENTAL FACTORS - Rosina

### Education:
 Children whose head-of-household has less than a high school degree

### Economic:
 Children in families on Public Assistance

### Cultural:
 Children in Immigrant Families

### Health:
 Children (<=17) without health insurance
 
 Breastfeeding, 2015

#### Sources for parental factors:
1. https://datacenter.kidscount.org/data#USA/2/0/char/0
2. https://www.kff.org/


## Project Report
## Extract
Our data formats:
CSV, XLSX

## Transform
Data cleaning using Pandas.

## Load
We decided to use a relational database because the information can be directly related to each other. We have worked with MySQL and SQLITE but chose SQLITE because we're working remotely/separately and its single-file storage format makes it easy to share.
