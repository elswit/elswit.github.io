+++
title = "Applied Stochastic Optimization"
description = "In antenna design"
date = 2014-11-18T02:13:50Z
author = "Arash Sarshar"
+++

## Array Pattern Synthesis Using stochastic optimizatin methods

In the most general context, the array Synthesis problem is finding the excitations 

<div> $$ a_{mn} e^{j \phi_{mn}} $$</div>

 of a one or two dimensional array of elements in a way that the overall radiation pattern approximates the ideal pre-defined radiation pattern or Gain specifications:

<div> $$ F(u,v)= \sum_{m,n} a_{mn} e^{j(mu+nv)}  \\ u=k_0 a \sin{\theta} \cos{\phi} \\  v=k_0 b \sin{\theta} \sin{\phi} $$ </div>




Often ideal radiation patterns fall into three basic categories: 

1. **Pencil Beam:** Used for direct *point-to-point* communications, antennas with pencil beam radiation patterns direct electromagnetic energy in a narrow spatial angle resulting in high gains in the boresight.
{{< figure src="../media/penc1.png" alt="A pencil beam radiation pattern" >}}
2. **Fan Beam:** Named after their fan-shaped radiation plots in polar coordinates, these patterns insure a roughly constant gain a wide angle that can be used in *point-to-multipoint* communications 
{{< figure src="../media/sqp_pat.png" alt="A fan beam radiation pattern" >}}
3. **Shaped Beam:** There are also cases in which a certain gain specifications is needed. One example is high altitude stationary satellites used for multimedia broadcasting over [specific geographical regions][pozar].

[pozar]:http://en.wikipedia.org/wiki/Geostationary_orbit


## Reflectarray Radiation Pattern Synthesis 

Reflectarray antennas are a hybrid form of antennas bringing the advantageous features of array antennas and reflector antennas together. Unlike conventional array antennas reflectarrays do not require complex feed circuitry inorder to radiate in predefiend radiation patterns. In reflectarray antennas a flat printed array of elements is illuminated by a source feed,  which is usually a small horn antenna. Each element receives the incident electromagnetic wave and re-radiates it with a certain phase shift. The overall reflectarray radiation pattern depends on the array factor, element radiation pattern and also the feed pattern. 
![Reflectarray antenna in antenna test chamber](../media/Reflectarray.png)
Various elements have been designed and employed for reflectarray antennas, ranging from stub-loaded patch elements, aperture coupled patches, loops, dipoles and ring elements.
In this [[paper]](http://ieeexplore.ieee.org/xpl/abstractAuthors.jsp?reload=true&tp=&arnumber=6546931) two novel elements are proposed: A stacked stub-loaded patch element for X-band linear polarization antenna with [True Time Delay] (http://scholar.google.com/scholar?hl=en&q=True+Time+Delay), and an aperture coupled patch  element  with  T-shaped  slots  for  dual  linear  or  circular  polarization  X-band reflectarray antenna. The performance of the elements is evaluated with the aid of full wave electromagnetic simulation software and the results are reported.
Also a new phase synthesis algorithm is developed for the radiation pattern synthesis of reflectarray antennas. Heuristic search methods are used for the synthesis of a shaped beam reflectarray and the efficiency of the methods are compared.




