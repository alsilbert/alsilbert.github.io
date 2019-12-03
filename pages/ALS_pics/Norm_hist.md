---
layout: frontpage
title: Normalized Wage and Number Histogram
---

<div class="navbar">
  <div class="navbar-inner">
      <ul class="nav">
          <li><a href="3d_kmeans_pay.html">prev</a></li>
          <li><a href="Full_SPLOM.html">next</a></li>
      </ul>
  </div>
</div>

[MatPlotLib's histogram function](https://matplotlib.org/3.1.1/api/_as_gen/matplotlib.pyplot.hist.html) is useful for gaining a basic visual understanding of our features.

![Normalized wage and number histogram](../../assets/ALS_pics/Norm_hist.png)

Given an apparent correlation between men's and women's pay, it is worth looking at this data in a different way that removes this inherent correlation. While it seems that pure numbers of women in an occupation does not make it more pay equitable, the differential in numbers between the genders may still have influence on the differential in pay. To test this, the data was manipulated to create two new variables: normalized pay differential and normalized number differential.

Neither element seems highly correlated with the other, a suspicion that was verified by their correlation coefficient of -0.156724. Moreover, the following histogram shows that the two elements do not even share a shape. The pay differential is a bell curve, while the number differential is not. The number differential does have a notable lean towards more occupations being populated by men than women -- interesting, but not for the current analysis.

The data for this analysis came from [“ACS 5-Year Estimates - Public Use Microdata Sample” for 2017 from the US Census Bureau](https://data.census.gov/mdat/#/) and from [Occupational Employment Statistics from the Bureau of Labor Statistics](https://www.bls.gov/oes/topics.htm#stem)
