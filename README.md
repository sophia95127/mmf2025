# MMF2025 Course Project - Robo Advisor

Updated on: July 6

Code have been done so far: We collect adjusted closed prices of:

1. Public equities: ZERA, GWW, etc.
2. Private equity: PSP
3. Fixed income: LQD, HYG
4. Real estate: IYR SYS
5. Risk fee rates: 3 month T-bill
6. Macro indicator: GDP, BCI, etc.
7. Benchmark: S&P 500

Group Member: Nan Cao, Fei Chen, Zhuoran Li, Keyu Wei, Bona Zhang

## Table of Contents

- [Background](#background)
- [Install](#install)

## Background
Today is June 1st 2021. We run a world-famous robo-advisor and received 5 years savings from a customer. The details of the savings are:

1. Initial capital: $100,000 CAD, provided on April 1st 2016
2. Injections of $10,000 CAD every 6 months, starting on October 1st 2016
3. Initial capital, and injections split 50/50 into USD and CAD (multi-currency)

**Portfolio Guidelines:**

1. Multi-asset portfolio (multi-currency): Equities, Fixed Income, Cash
2. Currency limits: currency mix should always remain between 40/60 – 60/40
3. Rebalancing: minimum every 6 months (must account for transaction costs)
4. Allowed up 20% of leverage

**Portfolio Construction/Strategy:**

1. Define portfolio construction/investment strategy – ideally use minimum 5 years of data to construct
2. Define risk characteristics of portfolio and validate
3. Back-testing: out-of-sample testing of models and portfolios before (before June 1st 2016)

**System designed to:**

1. Implement portfolio construction, back-testingand “automate” rebalancing
2. Portfolio analytics: exposures, performance, risk; breakdowns by currency, asset class, industry, etc...
3. Manage all the input and output data
4. Report: produce investor report (effectively communicate strategy, transactions, performance and risk)

![#1589F0](https://via.placeholder.com/15/1589F0/000000?text=+) **The goal for this repository are:**

1. Functions to organize input data (ETFs, economic indices, etc.). Calulate returns, risks, and covariance matrix.
2. An optimizer which involves gradient boosting machine learning algorithm to forecast future returns.
3. Different portfolio optimization functions.

## Install

This project uses cvxopt and xgboost. Go check them out if you don't have them locally installed.

```sh
$ pip install cvxopt
$ pip install xgboost
```

