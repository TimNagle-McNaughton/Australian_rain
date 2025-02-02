# Predicting rainfall at weather stations across Australia

Weather is a difficult dark art that many of us only notice when it is inaccurate. In 1963 Edward Lorenz published his pivotal paper ["Deterministic Nonperiodic Flow"](https://journals.ametsoc.org/downloadpdf/journals/atsc/20/2/1520-0469_1963_020_0130_dnf_2_0_co_2.xml)(PDF), most well-known in pop culture as 'the butterfly effect': complex systems are extremely sensitive to small changes in initial conditions. His findings caused him to question if long-term weather forecasting would ever be possible and feasible. 

Here we explore a more limited problem: how well can a random forest classifier predict if there was rain at a weather station today, or if there will be rain tomorrow? We test this question using ~10 years of records from 23 Australian weather stations that collect ~20 common weather metrics like temperature, humidity, air pressure, and wind speed/direction. Full definitions of all the features present in the dataset can be found [here](http://www.bom.gov.au/climate/dwo/IDCJDW0000.shtml). An example of what each of the ~140,000 records contain can be seen [here](http://www.bom.gov.au/climate/dwo/IDCJDW2801.latest.shtml). 

The random forests were generally very successful in predicting both same-day and next-day rainfall across Australia:

![Did it rain today?](https://github.com/TimNagle-McNaughton/Australian_rain/blob/main/Figures/Same-day_accuracy.png)

![Will it rain tomorrow?](https://github.com/TimNagle-McNaughton/Australian_rain/blob/main/Figures/Next-day_accuracy.png)
 
