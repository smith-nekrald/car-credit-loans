# Client Behavior on Car Credit Payments at a Bank in the Eastern Europe

This project addresses the problem of issuing a credit loan for the purpose of purchasing a car. 
The dataset was openly presented on a competition the author has opportunity to participate at 
by one of the Belarusian banks (more precisely, BNB-bank, or Belaruski Narodny Bank). This bank 
is specialized on medium-small business operations, industrial and personal loans, and is considered 
one of the most persistent links between the Republics of Belarus and Georgia. The main personal 
credit directions of BNB bank are car loans (9 credit lines) and mortgages (4 credit lines).

The competition was called Imaguru Datathon 2019, and was held in Minsk, Belarus
by Imaguru Startup Hub. After the dataset is revealed, the teams have 3 days to
complete their prototype and present for the jury. Note that it is somewhat a hobby
contest, not so much about prizes but more about networking and happy data science. The
dataset contains the payment history for several months, which is sometimes incomplete
and would be described in one of the next sections. Ideas studied in this project are in
part related to what was done at the time of the competition, as well as to the author’s
industrial experience.

The goal is to understand the client behavior and repayment policies based on their
internal features. Although credit scoring is working, clients behave differently. The natural
question is then how to use this variability in client behavior to make the bank better?
Note that financial atmosphere and economic ecology are very risky in Belarus, which adds
additional challenges to the problem.


## Structure of The Project:

The project is a POC (proof-of-concept) and is therefore implemented in Jupyter Notebook. To reproduce the results, it is important to run the notebooks
exactly in the following sequence:

**Step 1.** Notebook [1. initial-study.ipynb](https://github.com/smith-nekrald/car-credit-loans/blob/master/1.%20initial-study.ipynb) contains data exploration.

**Step 2.** Notebook [2. data-engineering.ipynb](https://github.com/smith-nekrald/car-credit-loans/blob/master/2.%20data-engineering.ipynb) implements feature engineering.

**Step 3.** Notebook [3. fit-clustering.ipynb](https://github.com/smith-nekrald/car-credit-loans/blob/master/3.%20fit-clustering.ipynb) fits clustering algorithms.

**Step 4.** Notebook [4. regress-next-months.ipynb](https://github.com/smith-nekrald/car-credit-loans/blob/master/4.%20regress-next-month.ipynb) fits next-period repayment prediction.

**Step 5.** Notebook [5. fill-nas-in-series.ipynb](https://github.com/smith-nekrald/car-credit-loans/blob/master/5.%20fill-nas-in-series.ipynb) fills NAs in time series for further clustering.

**Step 6.** Notebook [6. predict-clustering.ipynb](https://github.com/smith-nekrald/car-credit-loans/blob/master/6.%20predict-clustering.ipynb) clusters all time series.

**Step 7.** Notebook [7. client-reliability.ipynb](https://github.com/smith-nekrald/car-credit-loans/blob/master/7.%20client-reliability.ipynb) implements study of client reliability.


## Documentation
Project [report]() and corresponding [presentation]() are available in the `docs` subdirectory of the repository root.
