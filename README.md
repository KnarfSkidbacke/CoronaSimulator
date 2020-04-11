# CoronaSimulator
Simulation of corona virus infection (COVID-19) spreading over time (Cycles=days) and need for ICU (Intensive Care Unit), deathrate statistics.
Uses demographics data for Sweden 2019.
Uses html/javascript.

![alt text](https://github.com/KnarfSkidbacke/CoronaSimulator/blob/master/CoronaSim10.png)

## Simulation modell
A grid being a image bitmap is used to track the infection spreading. The actual infection growth is simulated by using a maxfilter over 4 closests gridcells to the gridcell to be processed. Also an social-contant-index value ranging from 0-2 is used to acount for the probalbility for an infection spread to occure.
The demographic data has a resolution of 1 year, which is cobined from data for men and women.

