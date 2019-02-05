+++
title = "Applied Stochastic Optimization"
description = "In fiber-optics filter design"
date = 2014-11-18T02:13:50Z
author = "Arash Sarshar"
+++

## Optical Filters based on a chain of Mach-Zehnder Interferometers 

### Mach-Zehnder Interferometer


[Mach-Zendher Interferometer][MZ] is an optical branch-line coupler. The input wave is directed in two separate optical paths, Therefore a relative phase shift is introduced that is proportional to the difference in the distance traveled by the wave. When the waves traveling in each optical pathway are coupled together again a diffraction pattern is produced at each output port. The power exiting each port is dependent on the path delay `$\Delta \tau$` and wavelength `$\lambda$`

![Mach-Zender interferometer schematic](../media/inter_schematic.png)

	
[MZ]: http://www.cs.princeton.edu/courses/archive/fall06/cos576/papers/zetie_et_al_mach_zehnder00.pdf

Cascading a number of M-Z interferometers with different charecteristics can make an optical filter. The overall filter transmission is the product of the transmission characteristics of each filter in the chain:

<div> $$ T(\nu)=\prod _i {T_i(\nu)}= \prod _i {\cos^2(\pi t_i \nu)}$$ </div>


## Design of Bandpass Optical Filters based on M-Z Interferometers

Optical filters are categorized as one the building blocks of optical networks. Many optical devices such as Multiplexers and De-multiplexers are based on optical filters. In a fiber communication network system, an optical filter can single out one or series of channels that are superimposed using wavelength division multiplexing in the in fiber. 
In practice, a cascade of Maach-Zehnder Interferometers can be fabricated as planar waveguides using Silica on Silicon technology.

Basic design parameters considered here are desired filter's center frequency and bandwidth. Since the design procedure is iterative, in each step the current design is compared with an ideal edge-sharp filter with the desired characteristics and a cost function is constructed. The Evolutionary Strategy Algorithm is then used to minimize this error.

## Results

Evolutionary Strategies (ES) is implemented with adaptive search sigma to design an optical filter based on 5 element cascade of Mach-Zehnder 


Filter Specifications     |    Minimum T     |    Maximum T      |      Number of      
--------------------------|:----------------:|:----------------: | ------------------- 
Center Frequency , BW (%)  |    nanosec.      |    nanosec.       |      M-Z elements
|          4 Thz, 10%         |      0.12     |         5         |           5          |


![example of a filter designed with ES](../media/Machres.png)

