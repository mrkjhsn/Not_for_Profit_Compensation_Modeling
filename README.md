## Predicting Executive Salary at Not-for-Profit Organizations

#### How much should a not-for-profit organization pay it's top management?  Not-for-profit organizations are devoted to myriads of causes and have a huge amount of variablity (mission, revenue, number of volunteers, ect.).  This makes predicting executive salary within these organizations a compelling challenge, and one that machine learning is well suited to make a contribution towards.

### Data source:

The data for this project was aquired from [Open990](https://www.open990.org/catalog/), an organization that aggregates and provides not-for-profit tax return data made public by the IRS.  Open990 also provides not-for-profit analytics services with this data for a [fee](https://appliednonprofitresearch.com/customdata/).  

These datasets have excellent documentation about what the attributes mean, and how the attributes have been mapped over from the 990 tax returns (Form 990, Form 990-EZ, Form 990-PF).  The executive compensation dataset provided by Open990 includes payments made to executives within the tax returns for years 2017 and 2018.

In addition to the executive compensation dataset, I used the governance dataset to get additional information about the governance of the organizations paying the executives in the executive dataset.  The governance dataset is mostly made up yes/no responses as to whether the not-for-profit has specific controls in place (conflict of interest policy, whistleblower policy, ect.)


### Motivations:

The IRS has [guidlines](https://www.irs.gov/charities-non-profits/exempt-organization-annual-reporting-requirements-meaning-of-reasonable-compensation) on compensation of top executives.  Specifically, it states "Reasonable compensation is the value that would ordinarily be paid for like services by like enterprises under like circumstances".  This leaves room for a wide latitude of interpretation.

Organizations filing a Form 990 are instructed to report compensation information for current (and some former) officers, directors, trustees, key employees (>150K), and five highest compensated (>100K) employees.

The United States has approximately 1.5M not-for-profit organizations.  Advocating for causes that are highly sympathetic, these organizations easily pull at the heartstrings of donors.  But how is that money being spent?

[Charity Navigator](https://www.charitynavigator.org/) has used a numbers-based rating system to score over 9,000 not-for-profits.  A model that could predict a reasonable salary executive salary could provide additional information to aid in their efforts to promote not-for-profit accountability.  

### Research questions:

1. Based on the unique characteristics of a not-for-profit, what should it be paying it's top executives?  
1. Is there a correlation between organizations with lax governance standards and disproportionate executive compensation?
1. Am I able to identify organizations who are likely paying their management more than they should?
