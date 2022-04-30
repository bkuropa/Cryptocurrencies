# Cryptocurrencies

A cryptocurrency is an encrypted data string that denotes a unit of currency. A network known as blockchain becomes an equivalent of the ledger for the currency and can be monitored through the same pathway.  Cryptocurrencies, Bitcoin being the best known style, are a relatively new method of transaction that is becoming more and more common in modern society including some cities allowing taxes and landlords allowing rents to be paid by this currency.  For the majority of people, it is not well understood and with the numerous currencies emerging all the time, those seeking to invest are unsure which direction to go.  Especially when Bitcoin itself is largely unaffordable.  

Analysis of accessable currency data, in this case through unsupervised learning, may make the comparison between currencies more understandable.  Principal Component Analysis (PCA) is attempted in combination with k-means clustering to better understand the groupings of the cryptocurrencies.

## Results
The current data under analysis is depicted in the table below before any processing is attempted:
![Crypto1](https://user-images.githubusercontent.com/19878877/166002565-2a157a53-0dfd-43ef-baf9-7bd6f90732f5.png)

Upon processing, 533 different cryptocurrencies are usable and 3 principal components are derrived for the initial analysis.
![PCA1](https://user-images.githubusercontent.com/19878877/166002590-baf52737-5a30-4b22-83bb-91b3832cb6ca.png)
The explained variance ratio of the components implies that 7% of the data is held in 3 PCAs but this may be due to the large number of extra columns (~90) holding 0s and 1s in addition to the major 2 financial columns.

In order to best optimized the k-means clustering technique, the following elbow curve is utilized to determine the best number of groups to divide into.  In this case the elbow is determined to be at point 3.
![bokeh_plot](https://user-images.githubusercontent.com/19878877/166002798-77c8ae96-6e9e-4359-9abc-01a26e7d1f65.png)

The different cryptocurrency styles can be observed in a number of ways.  Shown below are a 3D analysis and a dot plot.  One can notice the incredible difference between Bitcoin (Group 1) and all of the other currencies.  Due to its value and popularity, it appers as an intense outlier.
![3D_1](https://user-images.githubusercontent.com/19878877/166002835-2c8628d1-ef46-441d-bb9e-f0625b1d3e58.png)
![3D_2](https://user-images.githubusercontent.com/19878877/166002860-1b93388c-f56b-42a1-acc4-730e84525821.png)
![bokeh_plot (1)](https://user-images.githubusercontent.com/19878877/166002894-d7f8a47f-8bca-4f11-b0fd-11800665103d.png)
