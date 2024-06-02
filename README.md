# Insurance-Providers-and-Billing-Costs

# Project Overview
Research Question or Organizational Need
The project aims to examine whether there is a significant difference between the insurance
provider and billing amount for a synthetic healthcare dataset on Kaggle. The research question
is: “Does the insurance provider have a statistically significant effect on the billing amount?”
# Scope
The project focused on analyzing a synthetic healthcare dataset from Kaggle. The analysis
involved data cleaning, exploratory data analysis, statistical testing, and visualization. The scope
of the project was confined to the healthcare provider’s operations within the United States, and
it did not seek to apply the findings globally or to other countries. The analysis was based on the
assumption that the healthcare provider has multiple locations throughout the country.
# Overview of Solution
The project followed the Waterfall methodology, a linear and sequential approach that includes
Data Gathering and Cleaning, Data Analysis, Statistical Testing, and Visualization and
Reporting. The project used Jupyter Notebook as the development environment and several
Python libraries. The ydata_profiling library was used to create a profile report of the dataset.
The pandas library provided data structures and functions needed for data manipulation. The
matplotlib library was used for making static visualizations. The scipy library was used for
scientific computing and performing the Kruskal-Wallis H-test for independent samples. Lastly,
the seaborn library was used for creating appealing and informative statistical graphics.
# Project Plan
The project plan was executed as planned because the research question was well-defined and
the synthetic healthcare dataset from Kaggle was suitable for the analysis. The Python libraries
used were robust and provided all the necessary functions to clean the data, conduct the analysis,
and visualize the results. Notably, while the seaborn library was initially considered for use, it
was found that matplotlib sufficed for the visualization needs of the project and seaborn was not
needed for ydata_profiling to work. Therefore, seaborn was not utilized in this project. With
these tools and resources, the goals, objectives, and deliverables were met as planned.
# Project Planning Methodology
The project followed the Waterfall methodology. This linear and sequential approach began with
Data Gathering and Cleaning, followed by Data Analysis, Statistical Testing, and Visualization
and Reporting. Each phase was completed before proceeding to the next, ensuring a structured
and disciplined process. There were no variances in the project planning methodology because
the project was executed as planned following the Waterfall methodology.
# Project Timeline and Milestones
The project was broken down into four phases, each expected to take one day, with a total of 20
work hours spread across the phases. The timeline and milestones were met as planned, with no
variances. This was possible due to efficient work through any kinks or problems during the
analysis.
# Data Selection and Collection
The data selection and collection process did not differ from the plan because the synthetic
healthcare dataset was readily available on Kaggle. The dataset was in a CSV format, which is a
common data format that can be easily imported into most data analysis software for further
processing. The synthetic nature of the dataset, generated using Python’s Faker library, ensured
that it closely mimicked real-world healthcare data while maintaining privacy and
confidentiality. Therefore, there were no issues or changes in the data selection and collection
process.
# Handling Obstacles in Data Collection
There were no obstacles encountered while collecting the data because the dataset was of high
quality and complete. The dataset was already relatively clean, with no missing or null values in
any of the fields. The only data cleaning operation required was dropping duplicate entries. This
indicates that the dataset was well-prepared and suitable for analysis, eliminating potential
obstacles that often arise from dealing with messy or incomplete data.
# Handling Unplanned Data Governance Issues
There were no unplanned data governance issues because the dataset is synthetic and publicly
available on Kaggle, which eliminates major concerns regarding data privacy and security.
Advantages and Limitations of Data Set
One significant advantage of the dataset is its cleanliness and completeness. The dataset was
already relatively clean, with no missing or null values in any of the fields. This greatly
simplified the data preprocessing stage, allowing more time and resources to be devoted to the
analysis. For example, the absence of missing values in the dataset eliminates the need for
imputation or other techniques to handle missing data, which can introduce bias or inaccuracies
into the analysis. However, the dataset also has some limitations. One notable limitation is that it
is a synthetic dataset. While synthetic datasets are useful for maintaining privacy and
confidentiality, they may not perfectly represent real-world data. For instance, the synthetic
nature of the dataset means that it may lack some of the complexities and nuances found in
real-world healthcare data, such as outliers or unusual patterns. This could potentially limit the
generalizability of the findings to real-world scenarios.
# Data Extraction and Preparation
The data for this project was obtained from a synthetic healthcare dataset on Kaggle. The
extraction process involved downloading the dataset directly from Kaggle in a CSV (Comma
Separated Values) format. This format is widely used and can be easily imported into most data
analysis software for further processing. The use of a synthetic dataset, generated using Python’s
Faker library, ensured that the dataset closely mimicked real-world healthcare data while
maintaining privacy and confidentiality. This made the dataset suitable for a variety of data
analysis tasks. The extraction process was appropriate for the data because it allowed for easy
access and import of the data while preserving its integrity and confidentiality. The dataset used
for this project was already relatively clean, indicating its high quality. The only data cleaning
operation required was dropping duplicate entries in the dataset. In terms of completeness, each
field in the dataset was thoroughly checked for missing data. It was observed that there were no
fields with missing or null values, which signifies that the dataset is complete. Therefore, little to
no data preparation was necessary, which is not always the case with real-world data. This is
because real-world data often contains missing values, outliers, or errors that need to be
addressed during the data preparation stage. However, the high quality and completeness of this
synthetic dataset eliminated the need for extensive data preparation. The tools used for both data
extraction and preparation included Kaggle for data extraction and Python libraries for data
preparation. Python’s pandas library was used to import the CSV file and perform the data
cleaning operation of dropping duplicate entries. Given that the dataset is synthetic and publicly
available on Kaggle, there were no major concerns regarding data privacy and security.
# Data Analysis Methods
In the project, both descriptive and inferential statistics were employed for data analysis.
Descriptive statistics involved summarizing and organizing the data to present a clear picture of
the billing amounts across different insurance providers. Measures such as mean, median, mode,
and standard deviation were calculated to understand the central tendency and dispersion of
billing amounts. This step was crucial in understanding the basic features of the data and
providing a summary of the dataset. The main goal of inferential statistics was to test the
hypothesis that there would be no statistically significant difference in billing amounts among
different insurance providers. The Kruskal-Wallis test, a non-parametric test suitable for
comparing groups on a continuous variable when ANOVA assumptions are not met, was used for
this purpose. It checks the null hypothesis that the population median of all of the groups are
equal.
# Advantages and Limitations of Tools and Techniques
The project utilized several Python libraries, each with its own strengths and weaknesses.
Pandas, known for its robust data manipulation capabilities, was used, but it can be
memory-intensive for large datasets. Matplotlib offers flexibility for creating static
visualizations, yet it can be complex for advanced visualizations. Scipy provides a wide range of
functions for scientific computing, but it requires a good understanding of scientific computing
concepts. Seaborn, while user-friendly and compatible with Pandas dataframes, may not be as
flexible as Matplotlib for complex plots.
# Application of Analytical Methods
The data analysis process began with importing the necessary libraries, including
ydata_profiling, pandas, matplotlib, scipy, and scipy.stats. The synthetic healthcare dataset was
then loaded using pandas’ read_csv function. A profile report of the dataset was created using the
ProfileReport instance from ydata_profiling, which helped in understanding the structure,
relationships, and distributions in the dataset. The assumption that the dependent variable was
continuous was verified, and the samples were ensured to be independent by deleting duplicate
rows. A new CSV file with the cleaned data was created. The cleaned data was imported into
Tableau and box plots and histograms were created to verify the assumption that the data was
non-parametric and distributed relatively equally between the groups. Then, back in Jupyter
Notebook the data was grouped by insurance provider and the billing amount of each group was
retrieved as a numpy array. The arrays were unpacked and the Kruskal function was used to
obtain the test statistic and p-value. The test statistic was 1.5 and the p-value was 0.8. These were
compared to the alpha value of 0.05. Based on this comparison, it was concluded that the null
hypothesis failed to be rejected, suggesting that there is no significant statistical difference
between the billing amounts of the insurance providers.
# Statistical Significance
The null hypothesis for the project was that there is no significant statistical difference between
the billing amounts from the insurance providers. The Kruskal-Wallis test was used to test this
hypothesis. The metric generated from this test was the H-statistic, which was 1.5. The alpha
value, or the threshold for significance, was set at 0.05 or 5%. However, the p-value obtained
from the test was 0.8, which is greater than the alpha value. Therefore, there was not sufficient
evidence to reject the null hypothesis. This suggests that there is no significant statistical
difference between the billing amounts of the insurance providers.
# Practical Significance
In terms of practical significance, the results suggest that the insurance provider does not have a
significant impact on the billing amount. This could be meaningful in a real-world context, as it
could provide healthcare providers with assurance that the billing amounts are relatively
consistent across different insurance providers. This could allow them to focus their efforts on
other factors that might influence the billing amount. For example, a healthcare provider could
use this information to optimize their financial planning and budgeting processes, knowing that
the insurance provider does not significantly affect the billing amount.
# Overall Success
Overall, the project was successful in answering the research question and achieving its
objectives. The statistical analysis was conducted rigorously using an appropriate test, and the
results were interpreted accurately. The findings provided valuable insights into the relationship
between the insurance provider and the billing amount, which could have practical implications
for healthcare providers. Despite the null hypothesis not being rejected, the project was
successful in providing a clear and accurate understanding of the billing amounts across different
insurance providers.
# Conclusion
Summary of Conclusions
The project aimed to determine whether there is a significant statistical difference in billing
amounts among different insurance providers. The Kruskal-Wallis test was used to test this
hypothesis. The results indicated that there was not enough evidence to reject the null hypothesis,
suggesting that there is no significant statistical difference between the billing amounts of the
insurance providers. This conclusion is consistent with the dataset, chosen analytic methods, and
the stated goals of the project.
# Effective Storytelling
The findings of the project were communicated using visualizations created in Tableau,
including histograms and boxplots. Both the histogram and the boxplot effectively depicted the
spread of the billing costs between the insurance providers, providing a clear and intuitive way to
understand the distribution of billing amounts. These visualizations were designed to be
interactive, allowing for filtering by insurance providers. This interactivity enhanced the user’s
ability to explore and understand the data, supporting effective storytelling. The use of these
graphical representations visually conveyed the key findings of the analysis in an easily
understandable format. The tools used for the development of these visualizations, such as
Tableau, facilitated the creation of these dynamic and interactive visualizations, further
enhancing the storytelling process.
# Recommended Courses of Action
Since the insurance provider does not have a significant impact on the billing amount, the
healthcare provider could focus their efforts on other factors that might influence the billing
amount. This could involve examining patient demographics, specific medical procedures, or
other relevant factors. This recommendation directly addresses the research question by
suggesting alternative factors to consider in understanding variations in billing amounts.
Additionally, knowing that the insurance provider does not significantly affect the billing
amount, the healthcare provider could use this information to optimize their financial planning
and budgeting processes. This could involve adjusting their financial forecasts and budgets based
on the understanding that billing amounts are relatively consistent across different insurance
providers. This recommendation addresses the organizational need by suggesting ways to
leverage the findings for operational improvements.
