{
 "cells": [
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "## Reviewing Homework #4 Assigment 2: Xurui Chen, xc1454, Sherryairui"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "Xurui's null hypothesis:\n",
    "\n",
    "\"The number of old people who use citi bike is less than the number of young people\"\n",
    "\n",
    " _$H_0$_ :  $Age\\_above\\_45_{\\mathrm{count\\_day}} >= {Age\\_under\\_45_{\\mathrm{count\\_day}}}$\n",
    "\n",
    " _$H_1$_ :  $Age\\_above\\_45_{\\mathrm{count\\_day}} < {Age\\_under\\_45_{\\mathrm{count\\_day}}}$\n",
    "\n",
    "significance level  $\\alpha=0.05$\n",
    "\n",
    "which means i want the probability of getting a result at least as significant as mine to be less then 5%"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "**a. verify that their Null and alternative hypotheses are formulated correctly, and that they are state in both words and formulae (with the proper definitions to accompany the formulae)**\n",
    "\n",
    "This null hypothesis is stated in both words and formulae\n",
    "\n",
    "She also defines the significance level properly"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "**b. verify that the data supports the project: i.e. if the a data has the appropriate features (variables) to answer the question, and if the data was properly pre-processed to extract the needed values (there is some flexibility here since the test was not chosen yet)**"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "The data does not have the appropriate variables to test the null hypothesis as it is stated in words.  This would require a way to uniquely identify a person.  Instead Xurui seems to be analyzing the question stated in the formulae, which is whether more trips were made by old people vs young people, rather than whether more old or young people use citi bike, which should not depend on how much each person uses it."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "**c. chose an appropriate test to test _H0_ given the type of data, and the question asked.  You can refer to the flowchart of statistical tests for this in the slides, or [here](https://urldefense.proofpoint.com/v2/url?u=https-3A__www.ncbi.nlm.nih.gov_pmc_articles_PMC3116565_&d=DwIBAg&c=slrrB7dE8n7gBJbeO0g-IQ&r=FXpfbWDCNbAoPewUSOwlSA&m=kOCilXlvCMVIHNcu8TX5pspNtralYQR8Y74hmay8bgs&s=Sn0EdjZMwL5gIrzyahFavfphMwsPO7VVP5ZgWJ9mHes&e=), or the book Statistics in a Nutshell, or any of the resources that I shared in class.**"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "The question here is if there is an association between two variables: 1. old/young riders, and 2. ridership. The old/young rider vairable is ordinal, and therefore non-parametric. teh ridership variable has more than 2 categories, so the appropriate test here is a chi-square test for association."
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "**Write  your comments, suggestions, and suggested an appropriate statistical test, motivating your test choice, in a markdown **named CitibikeReview\\_\\<netID\\>.md**. Suggest variations on the question, if you think it may be made more interesting. **Do not perform the test yet.**"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "My suggestion is to restate the written null hypothesis so that it matches the formula version more directly.  This might be something like: \"The number of trips made by old people who use citi bike is less than the number trips made by young people\""
   ]
  },
  {
   "cell_type": "code",
   "execution_count": null,
   "metadata": {},
   "outputs": [],
   "source": []
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "PUI2016_Python3",
   "language": "python",
   "name": "pui2016_python3"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.5.4"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 2
}
