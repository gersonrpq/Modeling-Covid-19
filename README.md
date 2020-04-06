# Modeling Covid-19

<p align="center">
  <img src = "Images/example curves.png" height = "256">
</p>

Using data taken from https://ourworldindata.org/coronavirus-source-data

Two models are made to know the behavior of the CoVid-19 in every country. 
Once the logistic regression is made the amount of people infected at the end of the curve is calculated, and also when it would be the end of the CoVid-19 in a country.

To use it just run the function ```fit_and_plot_a_country``` with the country you want to know about.

```fit_and_plot_a_country```  could have the following parameters:

* ```country``` which means the name of the country as string, for example 'Spain'. Also there is a list of the countries that can be used in the notebook.
* ```src``` if you want to use your own dataset, this must be structured with a column with the date in the format ```2020-03-19``` and the name of the country with the total cases
* ```cases``` which means you want to know th beahavior of the total cases in a country if true, if false it evaluates deaths.
* ```p0_log``` first aproximation to make the logistic regression, it is a list like [5,73,20000]
* ```p0_exp``` first aproximation to make the exponential regression, it is a list like [1,1,1]
* ```predictions``` to make predictions if it is True
