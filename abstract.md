# Meteorologists and their CAPEs
## J.R. Leeman, R. May
### Unidata - Boulder, CO


#### Short Abstract
Meteorologists use the thermodynamic parameter convective available potential energy (CAPE) to help understand the severe weather potential of the atmosphere. Unfortunately, CAPE is calculated in a variety of ways, with corrections for virtual temperature, different adiabats, and different starting air parcels. We have implemented a robust, well tested, well documented, and easy to use set of thermodynamic calculations, including CAPE, in MetPy - the meteorological package for Python. We then show how one of the classic CAPE studies (Doswell and Rasmussen, 1994) can be reproduced quickly and in an interactive way with MetPy.

#### Background/Motivation
The thermodynamic parameter convective available potential energy (CAPE) is calculated from weather balloon (rawinsonde) observations and used to describe the energy available to fuel severe storms should convection occur. Calculation of CAPE appears deceptively simple. It is defined as the area between a theoretical parcel path and the observed environmental temperature. In practice there are numerous corrections, formulations of parcel paths, and types of CAPE discussed in the literature. Virtual temperature corrections can be used take into account the effects of water vapor on the gas constant and adiabats that include the ice phase transition are common variation. The parcel path can also be defined in different ways, including based on the surface observations, a mean of the mixed layer, or some other arbitrary starting point. We have designed a well-documented and easy to use set of meteorological calculations, including CAPE, in MetPy. We then use the package to reproduce a classic paper discussing the various flavors of CAPE (Doswell and Rasmussen, 1994).

#### Methods
We leverage the mathematical tools available in numpy and scipy, unit support from pint, and the current I/O capability of MetPy (https://github.com/Unidata/MetPy) to produce a tested and thorough CAPE calculation. MetPy is a meteorological data analysis and visualization package developed by the University Corporation for Atmospheric Research’s Unidata Program Center. We then use jupyter notebooks to reproduce the results of Doswell and Rasmussen (1994) showing the effects of employing or neglecting a virtual temperature calculation. With notebook widgets, the user can explore the data by creating custom date range queries, creating cross plots and histograms, and seeing summary statistics.  Analyses that took days of work when the paper was originally published can now be reproduced and even expanded in much less time.

#### Results
Our integration with existing tools, thorough unit testing, and thoughtful design result in functionality that is easy to use and that pulls back the curtain on the calculation methods employed in operational and research meteorology. The unit support removes user errors of providing quantities in the incorrect units and reduces the documentation workload. MetPy can be used to create both a research and teaching environment. Complex calculations can be easily performed to teach concepts in a class, but can also be deeply explored by advanced students. This tool chain can be carried away from the classroom and directly into graduate work or the workforce.

#### Conclusion
The scientific python tool chain, including domain specific libraries can be used to implement complex calculations with many variations in a sensible and well documented fashion. This functionality can aid reproducibility and bring professional tools to a level that can be used for classroom instruction and exploration.
Public Speaking Experience
John has extensive public speaking and conference participation experience. Conference presentations may be found on his website at http://www.johnrleeman.com/publications/. He presented at SciPy in 2016, with posters in 2014 and 2015.
