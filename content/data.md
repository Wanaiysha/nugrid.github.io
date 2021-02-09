# NuGrid Data Releases

## Set1/set1ext

* NuGrid data Set 1 consists of 2 metallicities, Z=0.01 (set 1.1) and Z=0.02 (set
1.2) ([Pignatari et al. 2016](http://adsabs.harvard.edu/abs/2016ApJS..225...24P)).  
* An extension of Set1 (Set1ext) adds three lower metallicites, as well as additional masses at all metallicities and MESA based massive star models for Z=0.01 and 0.02 ([Ritter et al. 2018](http://adsabs.harvard.edu/abs/2018MNRAS.480..538R)).
* An update of Set1 and Set1ext low-mass (M = 2 and 3 Msun) AGB models, called Set1upd, presents results with important updates for 3 metallicities already presented in Set1ext (Z=0.02, 0.01, 0.001), adding two new ones (Z=0.03 and Z=0.002). ([Battino et al. 2019](https://academic.oup.com/mnras/article/489/1/1082/5552141) and [Battino et al. 2021](https://www.mdpi.com/2218-1997/7/2/25)).

### Data access
* [Set 1 ext, DOI 10.11570/18.0002](https://www.doi.org/10.11570/18.0002)
* Access via the NuGrid Cyberhubs instance [WENDI](http://wendi.nugridstars.org)

See appendix of that paper for data access details. Please go to [Set 1](data-and-software/yields/set-1) of the Yields page in the [Yields Folder](data-and-software/yields), in the Data and software item on the left menu.

* Set1upd, Battino et al. 2019 (DOI:10.1093/mnras/stz2158) and Battino et al. 2021 (DOI:10.3390/universe7020025)
* Access via the [NuGrid Globus repository](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2F). From there, go in /data/set1upd/

### Yields tables

The Set 1 yield tables are provided at
[http://www.canfar.phys.uvic.ca/vosui/\#/nugrid/data/set1/Yield\_tables.](http://www.canfar.phys.uvic.ca/vosui/#/nugrid/data/set1/Yield_tables)

Set 1 extension yield tables together with a README file are provided at
<http://www.canfar.phys.uvic.ca/vosui/#/nugrid/data/set1ext/Yield_tables>

Set 1 updated yield tables, from both Battino et al. 2019 and 2021, are provided at
[https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1upd%2Fyields_finalabu_tables%2F](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1upd%2Fyields_finalabu_tables%2F)


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
Z=0.01 | <http://www.canfar.phys.uvic.ca/vosui/#/nugrid/data/set1ext/set1.1>
Z=0.006 | <http://www.canfar.phys.uvic.ca/vosui/#/nugrid/data/set1ext/set1.3a>
Z=0.001 | <http://www.canfar.phys.uvic.ca/vosui/#/nugrid/data/set1ext/set1.4a>
 Z=0.0001 |<http://www.canfar.phys.uvic.ca/vosui/#/nugrid/data/set1ext/set1.5a>

**Set 1 directories** 

Metallicity | Link
------------|-----
Z=0.02 | <http://www.canfar.phys.uvic.ca/vosui/#/nugrid/data/set1/set1.2>
Z=0.01 |<http://www.canfar.phys.uvic.ca/vosui/#/nugrid/data/set1/set1.1>


**Set 1 updated directories** 

Metallicity | Link
------------|-----
Z=0.03 | [LINK](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1upd%2Fset1.3%2F)
Z=0.02 | [LINK](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1upd%2Fset1.2%2F)
Z=0.01 | [LINK](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1upd%2Fset1.1%2F)
Z=0.002 |[LINK](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1upd%2Fset1.02%2F)
Z=0.001 |[LINK](https://app.globus.org/file-manager?origin_id=13897778-9894-11ea-b3c4-0ae144191ee3&origin_path=%2Fdata%2Fset1upd%2Fset1.01%2F)



### Figures

Data | Link
-----|-----
Set 1 | <http://www.canfar.phys.uvic.ca/vosui/#/nugrid/data/set1/Figures>
Set 1 extension | <http://www.canfar.phys.uvic.ca/vosui/#/nugrid/data/set1ext/Figures>

### References

- Ritter C, Herwig F, Jones S, Pignatari M, Fryer C, Hirschi R. 2018. MNRAS. 480(1):538–71 (Set 1 ext)
- Pignatari M, Herwig F, Hirschi R, Bennett M, Rockefeller G, et al. 2016. ASTROPHYS J SUPPL S. 225(2):24 (Set 1)
- Battino U., Tattersall A, Lederer-Woods C., Herwig F., Denissenkov P. et al.; MNRAS, 489, 1, 2019, 1082-1098, <https://doi.org/10.1093/mnras/stz2158> (Set 1 upd)
- Battino, U.; Lederer-Woods, C.; Cseh, B.; Denissenkov, P.; Herwig, F.; Universe 2021, 7, 25. <https://doi.org/10.3390/universe7020025> (Set 1 upd)
