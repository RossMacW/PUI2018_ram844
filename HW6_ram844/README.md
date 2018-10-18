# Assignment 1

### Reviewing Homework #4 Assigment 2: Xurui Chen, xc1454, Sherryairui"

Reviewed Xurui Chen's assignment and made pull request

Xurui's null hypothesis:

The number of old people who use citi bike is less than the number of young people\"\n",

_$H_0$_ :  $Age\\_above\\_45_{\\mathrm{count\\_day}} >= {Age\\_under\\_45_{\\mathrm{count\\_day}}}$\n",
_$H_1$_ :  $Age\\_above\\_45_{\\mathrm{count\\_day}} < {Age\\_under\\_45_{\\mathrm{count\\_day}}}$\n",

"significance level  $\\alpha=0.05$\n",

"which means i want the probability of getting a result at least as significant as mine to be less then 5%"

**a. verify that their Null and alternative hypotheses are formulated correctly, and that they are state in both words and formulae (with the proper definitions to accompany the formulae)**\n",

This null hypothesis is stated in both words and formulae\n",

She also defines the significance level properly"

**b. verify that the data supports the project: i.e. if the a data has the appropriate features (variables) to answer the question, and if the data was properly pre-processed to extract the needed values (there is some flexibility here since the test was not chosen yet)**"

The null hypothesis stated in words conflicts with teh null hypothesis sted in a formulae because their sign is different (\"less than\" in words but \">=\" in formula).


The data does not have the appropriate variables to test the null hypothesis as it is stated in words.  This would require a way to uniquely identify a person.  Instead Xurui seems to be analyzing the question stated in the formulae, which is whether more trips were made by old people vs young people, rather than whether more old or young people use citi bike, which should not depend on how much each person uses it."

**c. chose an appropriate test to test _H0_ given the type of data, and the question asked.  You can refer to the flowchart of statistical tests for this in the slides, or [here](https://urldefense.proofpoint.com/v2/url?u=https-3A__www.ncbi.nlm.nih.gov_pmc_articles_PMC3116565_&d=DwIBAg&c=slrrB7dE8n7gBJbeO0g-IQ&r=FXpfbWDCNbAoPewUSOwlSA&m=kOCilXlvCMVIHNcu8TX5pspNtralYQR8Y74hmay8bgs&s=Sn0EdjZMwL5gIrzyahFavfphMwsPO7VVP5ZgWJ9mHes&e=), or the book Statistics in a Nutshell, or any of the resources that I shared in class.**"

Since the citibike data does not provide data on individuals, you cannot test for the null hypothesis as stated in words.  However, you can test for the null hypothesis as stated in the formulae, so I am considering that here...

The question here is if there is an association between two variables: 1. old/young riders, and 2. ridership. The old/young rider vairable is nominal, and therefore non-parametric. The ridership variable has more than 2 categories, so the appropriate test here is a chi-square test for association."

**Write  your comments, suggestions, and suggested an appropriate statistical test, motivating your test choice, in a markdown **named CitibikeReview\\_\\<netID\\>.md**. Suggest variations on the question, if you think it may be made more interesting. **Do not perform the test yet.**"

My suggestion is to restate the written null hypothesis so that it matches the formula version more directly.  This might be something like: "The number of trips made by old people who use citi bike is less than the number trips made by young people"



# Assignment 2
worked with Mei Guan and Samantha Falk

Worked with Mei Guan @MeiGuan and Samantha Falk @samjfalk

Mei wrote the descriptions and we each picked one of the papers and created the table.

### ANOVA:
The paper  _[How accurate are runners’ prospective predictions of their race times?](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0200744)_ aimed to better understand prospective evaluations --being able to make an accurate prospective assessment of how one will perform on the annual half marathon race. The study looked at a variety of categorical variables such as demographics, gender, and prediction whilst controlling for experience levels via a categorical variable of running club membership. 

| **Statistical Analyses**	|  **IV(s)**  |  **IV type(s)** |  **DV(s)**  |  **DV type(s)**  |  **Control Var** | **Control Var type**  | **Question to be answered** | **_H0_** | **alpha** | **link to paper**| 
|:-------------------------:|:------------|:----------------|:------------|:-----------------|:-----------------|:--------------------- |:----------------------------|:--------:|:---------:|:-----------------|
|ANOVA	| 3, running club membership, gender, age | categorical | 1, interaction with prediction times| categorical | 1, experience measured via running club membership | categorical | How accurate are runner's prospective predictions of their finish running times?| Inexperienced runners predict as accurately as experienced runners. | 0.05 | [How accurate are runners’ prospective predictions of their race times?](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0200744) |

<img src="https://github.com/samjfalk/PUI2018_sjf374/blob/master/HW6_sjf374/Pics/ANOVA.png" width="500">

### Multiple Regression

The paper _[The Relationship between National-Level Carbon Dioxide Emissions and Population Size: An Assessment of Regional and Temporal Variation, 1960–2005](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0057107)_ investigates "the regional and temporal differences in the statistical relationship between national-level carbon dioxide emissions and national-level population size". The study analyzed panel data from 1960 to 2005 for a number of nations, used descriptive stats and regression modeling techniques.

|**Statistical Analyses**|  **IV(s)**  |  **IV type(s)** |  **DV(s)**  |  **DV type(s)**  |  **Control Var** | **Control Var type**  | **Question to be answered** | **_H0_** | **alpha** | **link to paper**| 
|:----------:|:----------|:------------|:-------------|:-------------|:------------|:------------- |:------------------|:----:|:-------:|:-------|
|Multiple Regression| 14, Population, Population 1965, Population 1970, Population 1975, Population 1980, Population 1985, Population 1990, Population 1995, Population 2000, Population 2005, GDP per capita, GDP per capita squared, Urban Population as Percent of Total Population, Trade as Percent of Total Gross Domestic Product| ratio | 1, Total Carbon Dioxide Emissions| ratio| 4, GDP per capita, GDP per capita squared, Urban Population as Percent of Total Population, Trade as Percent of Total Gross Domestic Product| ratio| What is the Relationship between National-Level Carbon Dioxide Emissions and Population Size| There is no relationship between the Population Size and the National-Level Carbon Dioxied Emissions. $H_0 : \beta_1 = 0$ | see Table 3 for beta coefficients and R squared in each of the 5 models | [The Relationship between National-Level Carbon Dioxide Emissions and Population Size: An Assessment of Regional and Temporal Variation, 1960–2005](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0057107) |


<img src="https://github.com/samjfalk/PUI2018_sjf374/blob/master/HW6_sjf374/Pics/multiple_regression.png" width="500">


### Logistic Regression

The paper _[Prediction of glycaemic control in young children and adolescents with type 1 diabetes mellitus using mixed-effects logistic regression modelling](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0182181)_ aims to identify patient characteristics that can be predictive of satisfactory glycaemic control in pediatric populations using a logistic regression.

| **Statistical Analyses**	|  **IV(s)**  |  **IV type(s)** |  **DV(s)**  |  **DV type(s)**  |  **Control Var** | **Control Var type**  | **Question to be answered** | **_H0_** | **alpha** | **link to paper**| 
|:----------:|:----------|:------------|:-------------|:-------------|:------------|:------------- |:------------------|:----:|:-------:|:-------|
Logistic Regression	| 3; HbA1c measurement, Age, fractional disease duration | Continuous | 1, the achievement of satisfactory glycaemic control | categorical | 0 | N/A | Which patient characteristics are predictive of satisfactory glycaemic control? | There is not a relationship between the independent variables and the achievement of satisfactory glycaemic control | N/A | [Prediction of glycaemic control in young children and adolescents with type 1 diabetes mellitus using mixed-effects logistic regression modelling](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0182181) |
  |||||||||

<img src="https://github.com/samjfalk/PUI2018_sjf374/blob/master/HW6_sjf374/Pics/Log_reg.PNG" width="500">



# Assignment 3
Worked with Mei Guan and Samantha Falk.  They helped me a lot.


# Assignment 4
Worked with Mei Guan and Samantha Falk.  They helped me a lot.