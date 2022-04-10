# Rossmann_sales_prediction
**Supervised Regression Machine Learning Capstone  Project**


Rossmann operates over 3,000 drug stores in 7 European countries. Currently, Rossmann store managers are tasked with predicting their daily sales for up to six weeks in advance. Store sales are influenced by many factors, including promotions, competition, school and state holidays, seasonality, and locality. With thousands of individual managers predicting sales based on their unique circumstances, the accuracy of results can be quite varied.
You are provided with historical sales data for 1,115 Rossmann stores. The task is to forecast the "Sales" column for the test set. Note that some stores in the dataset were temporarily closed for refurbishment.

# **Business Problem.**
The Rossmann Sales Company

**A private drug store chain based in Germany, with main operations on Europe. Operates over 3,000 drug stores in 7 different contries.
Offers heathcare and beauty product, including baby and body care, hygiene, cosmetics, dental hygiene, hair care, and so on.
Business Model: Product sales.**

**Problem**

The CFO wanted to reinvest in all stores, therefore, he need to know how much revenue each store will bring so he can invest it now.
Goal

**Predict the daily sales of all stores for up to six weeks in advance.**

# **Data Description**

**Rossmann Stores Data.csv** - historical data including Sales

**store.csv** - supplemental information about the stores

**Id**- an Id that represents a (Store, Date) duple within the test set

**Store** - a unique Id for each store

**Sales** - the turnover for any given day (this is what you are predicting)

**Customers** - the number of customers on a given day

**Open** - an indicator for whether the store was open: 0 = closed, 1 = open

**StateHoliday** - indicates a state holiday. Normally all stores, with few exceptions, are closed on state holidays. Note that all schools are closed on public holidays and weekends. a = public holiday, b = Easter holiday, c = Christmas, 0 = None

**SchoolHoliday** - indicates if the (Store, Date) was affected by the closure of public schools

**StoreType** - differentiates between 4 different store models: a, b, c, d

**Assortment** - describes an assortment level: a = basic, b = extra, c = extended

**CompetitionDistance** - distance in meters to the nearest competitor store

**CompetitionOpenSince[Month/Year]**- gives the approximate year and month of the time the nearest competitor was opened

**Promo** - indicates whether a store is running a promo on that day

**Promo2** - Promo2 is a continuing and consecutive promotion for some stores: 0 = store is not participating, 1 = store is participating

**Promo2Since[Year/Week]** - describes the year and calendar week when the store started participating in Promo2

**PromoInterval** - describes the consecutive intervals Promo2 is started, naming the months the promotion is started anew. E.g. "Feb,May,Aug,Nov" means each round starts in February, May, August, November of any given year for that store

# **Solution Strategy**
--
The strategy adopted was the following:

**Data Description:** I searched for NAs, checked data types (and adapted some of them for analysis) and presented a statistical description.

**Exploratory Data Analysis:** I performed univariate, bivariate and multivariate data analysis, obtaining statistical properties of each of them, correlations and testing hypothesis.

**Feature Engineering:** New features were created to make possible a more thorough analysis.

**Data Filtering:** Entries containing no information or containing information which does not match the scope of the project were filtered out.

**Data Preparation:** This step is necessary both for feature selection and for the machine learning models. Regarding the data types, numerical data was rescaled and categorical data was encoded.
