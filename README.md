# Brexit-vote-modelling
Brexit On June 23rd, 2016, The UK had a national referendum to decide whether the country should leave the EU (‘Brexit’). The result, a win for the Leave campaign, surprised many political commentators, who had expected that people would vote to Remain. Immediately people began to look for patterns that coud explain the Leave vote: cities had generally voted to Remain, while small towns had voted to Leave. England and Wales voted to Leave, while Northern Ireland and especially Scotland voted to Remain.

In the next few days, the Guardian newspaper presented some apparent demographic trends in the vote, based on the ages, incomes, education and class of different electoral wards (https://www.theguardian.com/politics/ ng-interactive/2016/jun/23/eu-referendum-live-results-and-analysis). The Guardian’s analysis stopped at showing these results graphically, and commenting on the apparent patterns. We will go one better by doing some real statistical analysis of the data.

I have scraped the data from the Guardian’s plots into a data file (brexit.csv).

There are 6 attributes in the data. The 5 possible input variables are:

abc1: proportion of individuals who are in the ABC1 social classes (middle to upper class) medianIncome: the median income of all residents medianAge: median age of residents withHigherEd: proportion of residents with any university-level education notBornUK: the proportion of residents who were born outside the UK These are normalised so that the lowest value is zero and the highest value is one. The output variable is called voteBrexit, and gives a TRUE/FALSE answer to the question ‘did this electoral ward vote for Brexit?’ (i.e. did more than 50% of people vote to Leave?).
