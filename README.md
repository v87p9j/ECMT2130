java c
ECMT2130 Financial Econometrics
Semester 2, 2024
GROUP PROJECT
DUE: 11.59pm Friday, 1st of November 2024
General Instructions
•    This is a group/individual assignment which accounts for 20% of your final mark. You are only
allowed to complete this assignment in groups if your name is registered in the group spreadsheet. The marking criteria will be the same, regardless of whether your work was done individually or   in groups.
•    Please type your answers (no handwriting). Make sure to compile all your answers in a single PDF file and submit it via Canvas.
•    There are 16 questions in this assignment. Please attempt all questions.
•    I will randomly select 5 questions to mark, and each question is worth 4 points. The total number of points of this assignment is therefore 20. The grading will be based on the completion and general quality of your submission.
•    Refer to the spreadsheet (link here) to find out which financial asset you or your group has been  allocated to. Failure to work with the correct series will result in loss of 10 marks and you might be referred to the Academic Integrity team.
•    Answer all questions in aneat PDF document (no other extensions accepted). Use Times New
Roman font size 12 throughout the report and normal margins. Make sure any images/screenshots included in the document are pasted in high definition: your report should look neat, clean, professional and easy to navigate. Failure to follow any of these instructions will result in a loss of 5 marks.
•    Only the group leader is required to submit the final report and other files. Please, make sure to
include a cover sheet with the SIDs of the group members, their signatures and the series assigned to the group. I made one available on the submission box. If you are completing the assignment individually, do the same but only with your information. Failure to include a complete cover sheet will incur in a penalty of 3 marks.
•    Based on University policy, a late submission is subject to a penalty of 5% (of the total points) per calendar day; and work submitted more than 10 days after the due date will receive a mark of zero.
•    You are required to work with R and Excel (no other software allowed). In addition to your report, you are required to submit your R script. and Excel spreadsheet. Include brief explanations of what you have done in both files (if we don’t understand what was done, we will consider it incorrect).
•    You should submit three files at most: (1) report in PDF format, (2) R script. and (3) Excel spreadsheet.
•    You are welcome to seek clarification/help from the teaching team, particularly with R and Excel. But the help will be naturally limited.PREPARATION
Each group/student is assigned a financial asset, probably a company listed in the Australian Stock Exchange (ASX). If you are part of a group,a ticker (a unique identification symbol    representing the company in the stock exchange) has already been assigned to you: it can be found on column G (named “ticker”) of the spreadsheet (link here).If you are doing the project individually, please fill in your information on the spreadsheet asap, so I can assign you a ticker. The earlier this process is completed the earlier you can  start working on your project.
Once you have been assigned a ticker, open the R script. (Data.R) and fill line 8 with your ticker. Follow line 9 as an example. Run the code and the result should be an Excel spreadsheet containing information on the asset price and the corresponding returns. Take sometime to familiarise yourself with the R script. provided.
You’re now ready to answer the questions.
QUESTIONS
Throughout the assignment,I will symbolise the series of (adjusted close) share price as pt and the corresponding series of returns with Rt. The timespan you should use is the one specified in the “Data.R” script. provided, i.e., from the 1st  of January 2021 until the 11th  of October 2024.
Using your assigned financial time series, answer the following questions:
1) Provide a brief overview of what the company you have been selected does. Make sure to include the goods/services it commercialises, number of clients, where it operates in the world, its main competitors and its last general financial figures. If you were given a commodity or a currency pair, make sure to include information on how important this commodity/currency is to the world and how muc代 写ECMT2130 Financial Econometrics Semester 2, 2024Processing
代做程序编程语言h money is commercialised.
Your answer should be around half a page: no more, no less.
2) If the Efficient Market Hypothesis (EMH) is true, do you expect to find a good model to forecast the conditional mean of pt  and Rt? Briefly explain.3) Plot pt. Make sure to include labels on they and x axes, as well as a title. Describe its  main features from a classical decomposition perspective. Hint: you might want to have a look at the lecture slides on this again.


4) Calculate the average, standard deviation, minimum, maximum, skewness and excess kurtosis of your series of prices and returns over the time span specified. Place them all on a neat table, preferably prepared in Excel (do not copy and pastethe R output). Interpret the excess kurtosis of your series.
5) Obtain a histogram for pt  and another one for Rt. Using the graphs and the basic statistics obtained in question 4, indicate whether the sampling distributions of price and return are visually normally distributed. Feel free to overlay a normal distribution on top of the histograms to strengthen your analysis and/or use statistical tests of normality.
6) Calculate the Sharpe ratio for Rt  and for the market proxy (ASX200 returns). You will    need to find the return of the risk-free asset for the relevant period. Briefly justify why you selected such a risk-free rate.
7) Calculate the alpha and beta of your assigned asset. Interpret both values. Do you have evidence pro or against the CAPM in your case? Use a hypothesis test to answer this question, making sure to indicate the null hypothesis of your tests in the explanation and considering a 5% significance level. Hint: be careful herewith the number of observations for both dependent and independent variables.
8) Using the data from 01/01/2021 until 01/03/2024 (training set), fit the following models to pt :
(i) Drift.
(ii) Mean.
(iii) Naïve.
Using the test set (data from 02/03/2024 until the last observed point), evaluate which model  fits the data best. Use the RMSE asthe criterion. Plot a graph of the series of prices and fitted values of your best model in the same picture. Forecast the next seven business days of data using your favourite model.
9) Fit the following modelstopt :
(i) Simple Exponential Smoothing (SES).
(ii) Holt’s linear trend.
(iii) Holt-Winters.Using the entire dataset here, which model fits the data better using the MAPE? Justify your choice. Forecast the next seven business days of data using your favourite model. Make sure to include 95% confidence intervals around the forecasts.
10) Is Rt  a stationary series? Use the plot of the returns, their ACF and the KPSS test to
justify your claim. Apply an appropriate level of differencing, if needed. If you do, show that the transformed series is now stationary using the KPSS test.


11) Using the ACF and PACF of the (potentially differenced) return series, propose a suitable ARIMA model. Explain how you obtained your answer and write out the model specification (equation). Compare this model with a simple model regressed on a constant only (with specification Rt  = μ + εt ). Use an information criterion of your choice to decide if your model is better than the simple model or not.
12) Using your preferred ARIMA model, produce forecasts for the next seven business days. Make sure to calculate the 95% forecasting intervals.
13) Using actual data from Yahoo Finance or equivalent, pick the model (from Q8, Q9 or Q11) that best forecasted the next five business days of Rt. Contrast this with what you expected in Q2.
14) Using Rt, propose an ARCH(1), ARCH(2) and ARCH(3) model. Are the parameter conditions met? Which one seems most appropriate for your data? Justify your answer. Plot the fitted variance of the returns.
15) Using Rt, propose a GARCH(1,1) model. Plot the fitted variance of the returns. Are the period(s) of high observed volatility in the graphs in Q3 consistent with the predicted volatility generated by the GARCH(1,1) model? Forecast the conditional variance for the next seven business days.
16) Assuming the return series follows a normal distribution, use the estimated mean and standard deviation you calculated in Q4 to estimate the 1%-VaR of your series. Produce forecasts for the 1%-VaR for the next seven business days using your best model for the  conditional mean and the conditional standard deviation.





         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
