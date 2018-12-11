# NuGrid Data Releases

## Set1/set1ext

* NuGrid data Set 1 consists of 2 metallicities, Z=0.01 (set 1.1) and Z=0.02 (set
1.2) ([Pignatari et al. 2016](http://adsabs.harvard.edu/abs/2016ApJS..225...24P)).  
* An extension of Set1 (Set1ext) adds three lower metallicites, as well as additional masses at all metallicities and MESA based massive star models for Z=0.01 and 0.02 ([Ritter et al. 2018](http://adsabs.harvard.edu/abs/2018MNRAS.480..538R)). 

### Data access
* [Set 1 ext, DOI 10.11570/18.0002](https://www.doi.org/10.11570/18.0002)
* Access via the NuGrid Cyberhubs instance [WENDI](http://wendi.nugridstars.org)

See appendix of that paper for data access details.Please go to [Set 1](data-and-software/yields/set-1) of the Yields page in the [Yields Folder](data-and-software/yields), in the Data and software item on the left menu.

### Yields tables

The Set 1 yield tables are provided at
[http://www.canfar.phys.uvic.ca/vosui/\#/nugrid/data/set1/Yield\_tables.](http://www.canfar.phys.uvic.ca/vosui/#/nugrid/data/set1/Yield_tables)

Set 1 extension yield tables together with a README file are provided at
<http://www.canfar.phys.uvic.ca/vosui/#/nugrid/data/set1ext/Yield_tables>

Documentation of how to extract table data can be found in [Analysis of
yield tables](../nugrid-data-server/analysis-of-yield-tables "Analysis of yield tables")

Note: In one safari browser version the links on this page did not
redirect properly to the canfar website. In this case we suggest to use
an alternative browser such as firefox.


### Stellar evolution and nucleosynthesis post-processing output

#### Directory structure for each metallicity on the CADC data server
In each of the metallicity directories the following data sets can be found:

   directory | data type
   ----------|------------
  see\_wind  | Stellar evolution output (pre-SN = wind) 
  see\_exp,  see\_exp\_yemcut   | Explosion data data, expl data assuming $Y_e$ cut
  ppd\_exp, ppd\_exp\_yemcut    | post-processing data of explosions (delayed and rapid), ppd of expl data assuming $Y_e$ cut
  ppd_wind    |   post-processing data of the pre-SN stellar evolution data see\_wind                             
                                       


**Set 1 extension directories**

These are the direct links to data directories on the CANFAR VOspace storage. This is the same data as the one referenced with the DOI given above.

Metallicity | Link
------------|-----
Z=0.02 | <http://www.canfar.phys.uvic.ca/vosui/#/nugrid/data/set1ext/set1.2>
Z=0.01 | <http://www.canfar.phys.uvic.ca/vosui/\#/nugrid/data/set1ext/set1.1>
Z=0.006 | <http://www.canfar.phys.uvic.ca/vosui/#/nugrid/data/set1ext/set1.3a>
Z=0.001 | <http://www.canfar.phys.uvic.ca/vosui/#/nugrid/data/set1ext/set1.4a>
 Z=0.0001 ||<http://www.canfar.phys.uvic.ca/vosui/#/nugrid/data/set1ext/set1.5a>

**Set 1 directories** 

Metallicity | Link
------------|-----
Z=0.02 | <http://www.canfar.phys.uvic.ca/vosui/#/nugrid/data/set1/set1.2>
Z=0.01 |<http://www.canfar.phys.uvic.ca/vosui/#/nugrid/data/set1/set1.1>

### Figures

Figures of Set 1 can be found at
[http://www.canfar.phys.uvic.ca/vosui/\#/nugrid/data/set1/Figures.](http://www.canfar.phys.uvic.ca/vosui/#/nugrid/data/set1/Figures)

Figures of Set 1 extension can be found at
[http://www.canfar.phys.uvic.ca/vosui/\#/nugrid/data/set1ext/Figures.](http://www.canfar.phys.uvic.ca/vosui/#/nugrid/data/set1ext/Figures)


### References
Ritter C, Herwig F, Jones S, Pignatari M, Fryer C, Hirschi R. 2018. MNRAS. 480(1):538–71 (Set 1 ext)
Pignatari M, Herwig F, Hirschi R, Bennett M, Rockefeller G, et al. 2016. ASTROPHYS J SUPPL S. 225(2):24 (Set 1)