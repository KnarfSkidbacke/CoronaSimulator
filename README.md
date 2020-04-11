# CoronaSimulator
Simulation of corona virus infection (COVID-19) spreading over time (Cycles=days) and need for ICU (Intensive Care Unit), deathrate statistics.
Uses demographics data for Sweden 2019.
Uses html/javascript.

![alt text](https://github.com/KnarfSkidbacke/CoronaSimulator/blob/master/CoronaSim10.png)

# Simulation modell
A grid being a image bitmap is used to track the infection spreading. 
<P>
The actual infection growth is simulated by using a maxfilter over 4 closests gridcells to the gridcell to be processed. Also an social-contant-index value ranging from 0-2 is used to acount for the probalbility for an infection spread to occure.
<P>
The demographic data has a resolution of 1 year, Sweden 2019 data, which is combined from data for men and women.
<P>
Each infected person is assumed to go thru incubation, sick and recovery cycle, which is being modelled using a sinus function. The positive sinus is when a perosn is infected then the sinus drops to negativ after the incubation, ther perosn becomes really sick. At the peak sickness level a randomfunction connects to the probability of age for death to be more likly for older people.

